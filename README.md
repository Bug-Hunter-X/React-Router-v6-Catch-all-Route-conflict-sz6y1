# React Router v6 Catch-all Route Conflict

This repository demonstrates a common issue in React Router v6 related to catch-all routes (`/*`).  When a catch-all route is placed before more specific routes, it can unintentionally intercept requests intended for those specific routes.  This can lead to unexpected rendering or routing behavior.

## Problem

The provided `App.js` uses a catch-all route (`/*`) to handle 404 errors. However, because it's placed before the other routes, it intercepts all requests, including those intended for `/` and `/about`. 

## Solution

The solution involves reordering the routes, placing the catch-all route (`/*`) last in the `Routes` component to handle any unmatched paths.

## Setup

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install dependencies.
4. Run `npm start` to start the development server.