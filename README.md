# React Router v6 useNavigate Hook Issue in Nested Components

This repository demonstrates a common issue encountered when using the `useNavigate` hook in React Router v6 within components that are not directly children of a route component. The navigation function may fail or behave unexpectedly if the component is conditionally rendered or deeply nested.

## Problem

The `useNavigate` hook relies on the router context. If the component where you are using it is not within the route hierarchy, the context might be unavailable, leading to errors or unexpected behavior.  This is frequently encountered with components rendered conditionally or many levels deep.

## Solution

The solution involves ensuring that the component using `useNavigate` is a part of the route tree or using a different approach like creating a context to provide the navigation functionality where it is needed.

## Setup

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install dependencies.
4. Run `npm start` to start the development server.