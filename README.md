# React Router v6 Catch-All Route Issue

This repository demonstrates a common issue encountered when using the catch-all route ('*') in React Router v6. The catch-all route, intended to handle all unmatched routes and display a 404 page, fails to render correctly in certain circumstances.

## Problem Description

The problem lies in how React Router v6 handles routes. The catch-all route should be the last route defined in your routes structure, to ensure that it only matches if no other routes match first.  If placed incorrectly, it may never get triggered.

## Solution

The solution is to ensure the catch-all route (`/*`) is placed as the last route within your `Routes` component. This guarantees that it only matches if no other routes match.  This example demonstrates the correct placement for the catch-all route.

## Setup

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.