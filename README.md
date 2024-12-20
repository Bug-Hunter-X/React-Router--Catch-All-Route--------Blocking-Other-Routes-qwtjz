# React Router Catch-All Route Bug

This repository demonstrates a common issue in React Router v6 where an incorrectly placed catch-all route (`/*`) prevents other routes from working as expected. The catch-all route will always be matched before other routes, causing issues in navigation.

## Problem:

When a catch-all route (`/*`) is placed before more specific routes, the catch-all route always matches, preventing the other routes from ever being reached.

## Solution:

The catch-all route should always be placed at the end of the route definitions within `Routes` in your React Router setup.