# 0x03. React Component

## Overview

This project involves working with React components, focusing on class components, lifecycle methods, event handling, higher-order components, and performance optimization. You'll be required to implement and test various React components and their functionalities.

## Learning Objectives

- Determine when to use a class or function to create a component.
- Understand the lifecycle of a class component.
- Test a component.
- Utilize a Jest spy to verify that a function is being called correctly.
- Explain what an HOC is and how to use it.
- Optimize performance and control which components to render.

## Requirements

- All files will be interpreted/compiled on Ubuntu 18.04 LTS using Node 12.x.x and npm 6.x.x.
- Allowed editors: `vi`, `vim`, `emacs`, `Visual Studio Code`.
- All files should end with a new line.
- A README.md file at the root of the project folder.

## Tasks

### 0. Commence with Class Components

Convert the `App` function into a React class in `App.js` from the last task of the `0x03. React Props` project. Ensuring tests are still passing.

- **Files:** `task_0/dashboard/src/App/App.js`
- **Repo:** `alx-react`
- **Directory:** `0x03-React_component`

### 1. Lifecycles

Add lifecycle methods to the `App` class, including an event listener to log out when `Ctrl + H` is pressed.

- **Files:** `task_1/dashboard/src/App/App.js`, `task_1/dashboard/src/App/App.test.js`
- **Repo:** `alx-react`
- **Directory:** `0x03-React_component`

### 2. Handling Events

Convert the `Notifications` component to a React class and add a `markAsRead` function.

- **Files:** `task_2/dashboard/src/Notifications/NotificationItem.js`, `task_2/dashboard/src/Notifications/NotificationItem.test.js`, `task_2/dashboard/src/Notifications/Notifications.js`, `task_2/dashboard/src/Notifications/Notifications.test.js`
- **Repo:** `alx-react`
- **Directory:** `0x03-React_component`

### 3. Reusable Components & Specialization

Create a `BodySection` component to handle containment of children elements.

- **Files:** `task_3/dashboard/src/BodySection/BodySection.js`
- **Repo:** `alx-react`
- **Directory:** `0x03-React_component`

### 4. Specialization

Create a `BodySectionWithMarginBottom` component with specific styles.

- **Files:** `task_3/dashboard/src/BodySection/BodySectionWithMarginBottom.js`, `task_3/dashboard/src/BodySection/BodySection.css`
- **Repo:** `alx-react`
- **Directory:** `0x03-React_component`

### 5. Use the New Components

Modify the `App` component to use `BodySectionWithMarginBottom` and `BodySection`.

- **Files:** `task_3/dashboard/src/App/App.js`
- **Repo:** `alx-react`
- **Directory:** `0x03-React_component`

### 6. Test the New Components

Add tests for `BodySection` and `BodySectionWithMarginBottom`.

- **Files:** `task_3/dashboard/src/BodySection/BodySection.test.js`, `task_3/dashboard/src/BodySection/BodySectionWithMarginBottom.test.js`
- **Repo:** `alx-react`
- **Directory:** `0x03-React_component`

### 7. Create WithLogging HOC

Create a HOC named `WithLogging` to log component mounting and unmounting.

- **Files:** `task_4/dashboard/src/HOC/WithLogging.js`
- **Repo:** `alx-react`
- **Directory:** `0x03-React_component`

### 8. Write a Test for the HOC

Write tests for the `WithLogging` HOC to ensure it logs correctly.

- **Files:** `task_4/dashboard/src/HOC/WithLogging.test.js` 