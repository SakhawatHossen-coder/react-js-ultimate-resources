## Create your project

Start by creating a new Vite project if you don’t have one set up already. The most common approach is to use Create Vite.
Terminal

    npm create vite@latest my-project -- --template react
    cd my-project

Install Tailwind CSS

Install tailwindcss and its peer dependencies, then generate your tailwind.config.js and postcss.config.js files.
Terminal

    npm install -D tailwindcss postcss autoprefixer
    npx tailwindcss init -p

    Configure your template paths

Add the paths to all of your template files in your tailwind.config.js file.
tailwind.config.js

    /** @type {import('tailwindcss').Config} */
    export default {
    content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
    ],
    theme: {
    extend: {},
    },
    plugins: [require("daisyui")],
    }

Add the Tailwind directives to your CSS

Add the @tailwind directives for each of Tailwind’s layers to your ./src/index.css file.
index.css

    @tailwind base;
    @tailwind components;
    @tailwind utilities;

## Daisy Ui

Install daisyUI:

    npm i -D daisyui@latest

## React

React-Toastify allows you to add notifications to your app with ease. No more nonsense!
Installation

    npm install --save react-toastify

## React Project Resources

This document provides a central hub for essential links to popular React libraries and tools that can enhance your project's functionality and style.

Styling Libraries:

    Tailwind CSS

(https://tailwindcss.com/docs/installation):

     A utility-first CSS framework that streamlines the creation of responsive layouts and components without writing extensive CSS classes.
    DaisyUI

(https://daisyui.com/):

     A component library built on top of Tailwind CSS, offering pre-designed components for buttons, forms, navigation, and more, to accelerate your development process.

UI Notifications:

    React Toastify

(https://github.com/fkhadra/react-toastify):

     A flexible library for displaying customizable user notifications (toasts) in your React applications, ideal for providing feedback and alerts.

Database Integration:

Firebase (https://firebase.google.com/):

    Google's cloud-hosted platform offering various backend services, including authentication, databases (Real-time Database and Firestore), cloud storage, hosting, and more. Firebase streamlines backend integration and data management for your React apps.

Routing:

React Router

(https://reactrouter.com/en/main/start/tutorial):

    npm install react-router-dom localforage match-sorter sort-by

A powerful routing library for managing navigation and URL structures within your React applications. It enables you to easily create single-page applications (SPAs) with smooth transitions between different views.

Icons:

React Icons

    https://react-icons.github.io/react-icons/
    npm install react-icons --save

A collection of popular icon packs integrated as React components, making it simple to incorporate beautiful and diverse icons into your React interfaces.

Additional Resources:

    React Official Documentation (https://legacy.reactjs.org/docs/getting-started.html): The definitive resource for learning React, covering core concepts, APIs, best practices, and more.
    React Bootstrap (https://github.com/react-bootstrap/react-bootstrap): Another popular UI component library built on top of Bootstrap for those familiar with the Bootstrap framework.
