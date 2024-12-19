# React Router v6 Catch All Route Issue

This repository demonstrates a problem with the catch-all route (`/*`) in React Router v6.  The catch-all route is intended to handle any unmatched routes, but in this example, it does not function correctly.

## Problem

When navigating to a route that doesn't exist, the `NotFound` component is not rendered as expected.  The application instead displays nothing.

## Solution

The solution involves ensuring the catch-all route is placed last in the `Routes` component. The order of routes is significant in React Router v6, and placing the catch-all route before other routes causes conflicts.  See the `AppSolution.js` file for a corrected implementation.
