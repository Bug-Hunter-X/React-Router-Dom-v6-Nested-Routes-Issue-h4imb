# React Router Dom v6 Nested Routes Issue

This repository demonstrates a common issue encountered when working with nested routes in React Router Dom v6.  The problem arises when trying to navigate directly to a child route; it will not render correctly, even though the parent route does render.  The child route only renders if you first navigate to the parent and then to the child route.

## Problem Description

The provided code uses nested routes to create a simple navigation structure. When navigating directly to `/contact/form`, the `ContactForm` component does not render. However, if you first navigate to `/contact`, then to `/contact/form`, the `ContactForm` will render correctly. This is a common problem often overlooked when working with nested routes in React Router v6.

## Solution

The solution involves adding an index route to the parent route to force a render.
