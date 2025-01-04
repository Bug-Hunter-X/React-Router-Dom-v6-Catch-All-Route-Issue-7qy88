# React Router Dom v6 Catch-All Route Issue

This repository demonstrates a problem with the catch-all route (`/*`) in React Router Dom v6.  The catch-all route is intended to match any URL that doesn't match other defined routes, effectively creating a 404 page. However, in this example, the catch-all route is being ignored.  The solution provided demonstrates a correct way to implement the catch-all route for optimal functionality.

## Problem

The issue lies in the order and specificity of routes within the `Routes` component.  The catch-all route (`/*`) needs to be placed at the end of your route definitions. Other routes with more specific paths will always take precedence if placed above the catch-all route.