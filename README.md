#  React + Vite Setup Guide

A clean and minimal template to run **React with Vite**, including **Hot Module Replacement (HMR)** and basic **ESLint configuration** for modern frontend development.

---

#  About This Template

This template provides the fastest way to start a React project using **Vite**, which offers:

-  Instant dev server startup  
-  Hot Module Replacement (HMR)  
-  Optimized production builds  
-  ESLint support  

---

#  Official React Plugins for Vite

Currently, two official plugins are available:

### 1️ React Plugin (Babel)

Uses **Babel** for Fast Refresh.

Plugin: `@vitejs/plugin-react`  
Repo: https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react  

Technologies used:

- Babel → https://babeljs.io/  
- OXC (when used in Rolldown Vite) → https://oxc.rs  

---

### 2️ React Plugin (SWC)

Uses **SWC**, a faster Rust-based compiler.

Plugin: `@vitejs/plugin-react-swc`  
Repo: https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc  

SWC website:  
https://swc.rs/

---

#  React Compiler

The **React Compiler** is not enabled in this template because it can affect development and build performance.

If you want to enable it, follow the official documentation:

https://react.dev/learn/react-compiler/installation

---

#  Expanding the ESLint Configuration

For **production applications**, it is recommended to use:

- **TypeScript**
- **Type-aware lint rules**

You can use the official React + TypeScript Vite template:

https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts

You can also integrate:

`typescript-eslint`  
https://typescript-eslint.io

---

#  React Installation — Step by Step Guide

---

# 1️ Install Node.js

Download the **Node.js LTS version**

https://nodejs.org

After installing, verify installation in the terminal:

node -v  
npm -v  

If installed correctly, the terminal will show version numbers.

---

# 2️ Create a React Project (Using Vite)

Run the following command:

npm create vite@latest

Answer the prompts:

Project name: my-react-app  
Framework: React  
Variant: JavaScript  

---

# 3️ Go into the Project Folder

cd my-react-app

---

# 4️ Install Dependencies

npm install

This installs all required project packages.

---

# 5️ Start the React Development Server

npm run dev

The terminal will show something similar to:

VITE ready in 300ms  
Local: http://localhost:5173/

Open the link in your browser.

---

#  React Project Structure

my-react-app

│  
├── node_modules  
├── public  

├── src  
│   ├── assets  
│   ├── App.jsx  
│   ├── main.jsx  
│   └── index.css  

├── package.json  
├── vite.config.js  
└── index.html  

---

#  Editing the React Page

Open the file:

src/App.jsx

Example code:

function App() {
  return (
    <h1>Hello React </h1>
  )
}

export default App

After saving the file, the browser will automatically refresh because of **HMR**.

---

# Install Common React Libraries (Optional)

React Router (for routing)

npm install react-router-dom

Axios (for API requests)

npm install axios

Tailwind CSS (for styling)

npm install -D tailwindcss postcss autoprefixer  
npx tailwindcss init -p

---

#  Build Project for Production

Run:

npm run build

Production files will be generated in:

dist/

These files are ready for deployment.

---

#  Quick Installation Commands

For faster setup:

npm create vite@latest my-react-app  
cd my-react-app  
npm install  
npm run dev

---

#  Summary

Using **React + Vite** provides:

 Extremely fast development  
 Instant updates with Hot Module Replacement  
 Optimized production builds  
 Linting support  
 Clean project structure  

It is one of the best setups for building **modern React applications**.
