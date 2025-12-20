# ReactGuard: Mastering Error Handling

## Project Overview

ReactGuard is a Next.js project that focuses on implementing robust error handling using React Error Boundaries. The goal of this project is to ensure that runtime JavaScript errors do not crash the entire application, while still providing a clean user experience and proper error monitoring.

The project demonstrates how to build an ErrorBoundary class component in TypeScript, integrate it into a Next.js app, test it using an intentionally failing component, and log errors using Sentry.

---

## Project Information

- Project Name: ReactGuard: Mastering Error Handling
- Weight: 1
- Start Date: December 15, 2025
- End Date: December 22, 2025
- Review Type: Manual QA Review

Important: Submitting after the deadline will prevent you from generating a review link.

---

## Learning Objectives

By completing this project, you will be able to:

- Understand how React Error Boundaries work
- Implement a class-based React component using TypeScript
- Handle runtime errors gracefully in a Next.js application
- Integrate third-party error monitoring tools
- Test and validate error-handling components

---

## Key Concepts

- Error Boundaries  
  React components that catch JavaScript errors in their child component tree.

- Component Lifecycle Methods  
  Using getDerivedStateFromError and componentDidCatch to handle errors.

- Fallback UI  
  Displaying a user-friendly message instead of a broken application.

- Error Recovery  
  Allowing users to retry after an error occurs.

- Error Monitoring  
  Logging and tracking errors using services like Sentry.

---

## Tools and Technologies

- React
- Next.js
- TypeScript
- Sentry
- Node.js / npm

---

## Real-World Use Case

Error boundaries are essential in production applications because they:

1. Prevent the entire application from crashing due to a single component failure
2. Provide meaningful feedback instead of blank screens
3. Capture and log errors for debugging
4. Allow recovery from non-critical failures
5. Improve overall application stability and user experience

This pattern is widely used in large-scale web applications to ensure reliability and maintainability.

---

## Project Structure

alx-rick-and-morty-app/
├── components/
│   ├── ErrorBoundary.tsx
│   └── ErrorProneComponent.tsx
├── pages/
│   ├── _app.tsx
│   └── index.tsx
├── package.json
└── README.md

---

## Implementation Summary

### Task 0: Create the ErrorBoundary Component

- Created an ErrorBoundary class component using TypeScript
- Implemented state tracking with hasError
- Used getDerivedStateFromError to update state when an error occurs
- Used componentDidCatch to capture error details
- Displayed a fallback UI with a “Try again” button

### Task 1: Wrap the Application with ErrorBoundary

- Imported the ErrorBoundary into pages/_app.tsx
- Wrapped the main Component with ErrorBoundary
- Ensured all pages are protected from runtime errors

### Task 2: Create a Component to Test ErrorBoundary

- Created ErrorProneComponent that throws an error on render
- Imported and rendered the component inside ErrorBoundary
- Verified that the fallback UI appears when an error occurs

### Task 3: Monitor and Log Errors

- Installed Sentry SDK
- Integrated Sentry inside componentDidCatch
- Confirmed errors are logged in the Sentry dashboard

---

## How to Run the Project

1. Clone the repository:
   git clone https://github.com/<your-username>/alx-graphql-0x03.git

2. Navigate to the project directory:
   cd alx-graphql-0x03/alx-rick-and-morty-app

3. Install dependencies:
   npm install

4. Start the development server:
   npm run dev

5. Open your browser and visit:
   http://localhost:3000

---

## Testing the Error Boundary

- Load the page that renders ErrorProneComponent
- Confirm the fallback UI is displayed
- Click the “Try again” button to reset the error state
- Check the Sentry dashboard to verify error logging

---

## Assessment Notes

This project is evaluated primarily through manual review.

To receive full credit:
- Complete all mandatory tasks
- Submit all required files
- Generate your review link before the deadline
- Complete peer reviews

An automated check will verify the presence of required core files.

---

## Author

Laughter Webs

---

Happy coding. This project demonstrates real-world error handling patterns used in production React and Next.js applications.
