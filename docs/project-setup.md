# React Interactive Google Maps POC - Setup Guide

This document outlines the steps to set up and run the React Interactive Google Maps Proof of Concept project.

## Initial Project Setup

1. Create a new React project using Create React App with the CRA template:

   ```bash
   npx create-react-app react19-interactive-google-maps-poc --template cra-template
   cd react19-interactive-google-maps-poc
   ```

   This will create a new React project with the following features:

   - React and ReactDOM
   - React Scripts
   - Git repository initialized
   - Development dependencies configured

2. Available Scripts:

   - `npm start`: Starts the development server
   - `npm run build`: Bundles the app for production
   - `npm test`: Starts the test runner
   - `npm run eject`: Ejects from Create React App (one-way operation)

3. Clean up the initial project structure:
   - In `src/App.js`:
     - Remove the default logo import
     - Clear the default content in the App component
     - Keep only the basic component structure
   - In `src/App.css`:
     - Remove the default styling and App logo animation
     - Keep only the necessary styles
   - In `src/index.js`:
     - Keep the React and ReactDOM imports
     - Keep the App component import
     - Keep the root rendering logic
   - Files to keep:
     - `src/index.js` - The application entry point
     - `src/App.js` - The main App component
     - `src/App.css` - Main application styles
     - `src/index.css` - Global styles
     - `public/index.html` - HTML template
   - Files that can be removed:
     - `src/logo.svg` - Default CRA logo
     - `src/App.test.js` - Default test file
     - `src/setupTests.js` - Test configuration
     - `src/reportWebVitals.js` - Performance measuring
     - `public/logo192.png` and `public/logo512.png` - Default icons

## Installing Dependencies

1. Install the Google Maps React wrapper library:

   ```bash
   npm install @react-google-maps/api
   ```

## Project Structure

The project follows a standard React application structure:

```plaintext
├── public/
│   ├── favicon.ico
│   ├── index.html
│   ├── logo192.png
│   ├── logo512.png
│   ├── manifest.json
│   └── robots.txt
├── src/
│   ├── App.css
│   ├── App.js
│   ├── App.test.js
│   ├── index.css
│   ├── index.js
│   ├── logo.svg
│   ├── reportWebVitals.js
│   └── setupTests.js
├── package.json
└── README.md
```

## Running the Application

1. Install all dependencies:

   ```bash
   npm install
   ```

2. Start the development server:

   ```bash
   npm start
   ```

The application will be available at `http://localhost:3000`

## Notes

- Make sure you have Node.js and npm installed on your system
- You'll need to obtain a Google Maps API key to use the maps functionality
- The project uses React features from Create React App template
- Initial setup may show some npm funding requests and vulnerabilities
  - Run `npm audit fix --force` to address vulnerabilities if needed
- A git repository is automatically initialized with an initial commit
