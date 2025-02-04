# Next.js 15 Runtime Error in Page Component

This repository demonstrates a runtime error in a Next.js 15 application that is not properly handled.

## Issue

A runtime error occurs in the `pages/about.js` component due to accessing an undeclared variable. This results in a blank page instead of a helpful error message to the user.

## Setup

1. Clone this repository.
2. Navigate to the project directory `cd nextjs-runtime-error`.
3. Install dependencies: `npm install`
4. Run the development server: `npm run dev`

## Reproduce

Navigate to `/about` in your browser. You'll see a blank page.  The console will display a JavaScript error indicating that `nonexistentVariable` is not defined.

## Solution

The `aboutSolution.js` file provides a solution implementing error boundaries to gracefully handle this type of runtime error.

## How to fix

Add proper error handling in your components or utilize error boundaries to gracefully catch and display user-friendly error messages.