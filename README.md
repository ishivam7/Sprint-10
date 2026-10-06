# Sprint - 10  E-Commerce Redux Migration 

A fully functional, state-driven e-commerce application built for the Assignment 1 engineering requirements. This project focuses on migrating global state management from Context API to Redux Toolkit (RTK), featuring dynamic cart calculations and optimized event handling.

## Important Links

- **Live Website:** https://sprint-10-one.vercel.app/


### Tech Stack

- **React (Vite)**
- **Redux Toolkit (@reduxjs/toolkit)**
- **React-Redux**
- **React Router DOM**
- **Data Source:** `dummyjson.com` API

### Features Completed

- **Global Store Architecture:** Successfully completely migrated from Context API to Redux Toolkit, setting up a centralized store (`store.js`) and wrapping the app with `<Provider>`.
- **Redux Slices:** Implemented `cartSlice` to manage adding products and updating quantities, and `filterSlice` to handle product category filtering.
- **Smart Navbar:** Features a dynamic shopping cart counter that calculates the total number of items in real-time using `useSelector` and the `.reduce()` array method.
- **Interactive Product Cards:** Features a functional "Add to Cart" button that dispatches Redux actions.
- **Event Delegation Handling:** Implemented `e.stopPropagation()` on the Add to Cart button to prevent unwanted event bubbling and route navigation when users interact with the cart button.
