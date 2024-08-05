# 0x09 React Redux Connectors and Providers

## Project Overview

This project focuses on integrating Redux with React components using connectors and providers. You'll work with Redux to manage application state, connect components, and utilize middleware for async actions. By the end of this project, you'll have a solid understanding of Redux connectors, providers, and performance optimization techniques.

## Learning Objectives

By completing this project, you should be able to:

- Explain Redux connectors and their usage.
- Understand and use `mapStateToProps` and `mapDispatchToProps`.
- Connect action creators to components, including async actions with Redux Thunk.
- Configure Redux Providers and set up the app’s store.
- Improve connector performance with Reselect.
- Debug using Redux DevTools.

## Project Details

- **Start Date:** August 1, 2024, 5:00 AM
- **End Date:** August 8, 2024, 5:00 AM
- **Checker Release Date:** August 2, 2024, 11:00 PM
- **Auto Review Deadline:** August 8, 2024, 5:00 AM

## Requirements

- **Allowed Editors:** vi, vim, emacs, Visual Studio Code
- **Files:** All files must end with a new line.
- **README.md:** A `README.md` file is mandatory at the root of your project folder.
- **Environment:** The project will be interpreted/compiled on Ubuntu 18.04 LTS using Node 12.x.x and npm 6.x.x.
- **Push:** Ensure all files, including `package.json` and `.babelrc`, are pushed to the repository.
- **Functions:** All functions must be exported.

## Provided Files

- `dashboard/dist/courses.json`
- `dashboard/dist/login-success.json`
- `dashboard/dist/notifications.json`

## Tasks

### 0. Write `mapStateToProps`

- **File:** `task_0/dashboard/src/App/App.js`
- **Description:** Create a `mapStateToProps` function to connect `uiReducer` and the `isLoggedIn` property to your component.

### 1. Create a Small Store

- **File:** `task_0/dashboard/src/index.js`
- **Description:** Create a store using `createStore` and pass it to the main App via a Provider.

### 2. Test `mapStateToProps`

- **File:** `task_0/dashboard/src/App/App.test.js`
- **Description:** Export `mapStateToProps` and create a test suite to verify its functionality.

### 3. Update `mapStateToProps`

- **File:** `task_1/dashboard/src/App/App.js`
- **Description:** Update `mapStateToProps` to include `displayDrawer` and connect it to the `isNotificationDrawerVisible` attribute.

### 4. Connect Your Action Creators

- **File:** `task_1/dashboard/src/App/App.js`
- **Description:** Connect `displayNotificationDrawer` and `hideNotificationDrawer` action creators to your component.

### 5. Refactor Your Code

- **File:** `task_1/dashboard/src/App/App.js`
- **Description:** Refactor the code by removing old methods and setting up `propTypes` and `defaultProps`.

### 6. Update Your Tests

- **File:** `task_1/dashboard/src/App/App.test.js`
- **Description:** Refactor tests to remove outdated tests and update for new attributes.

### 7. Async Actions & Thunk Middleware

- **File:** `task_2/dashboard/src/index.js`
- **Description:** Install `redux-thunk` and apply middleware to your store for handling async actions.

### 8. Connect `loginRequest` to the App

- **File:** `task_2/dashboard/src/App/App.js`
- **Description:** Connect `loginRequest` action creator and refactor the component accordingly.

### 9. Connect User State to the Footer

- **File:** `task_2/dashboard/src/Footer/Footer.js`
- **Description:** Create a `mapStateToProps` function for the `Footer` component and connect it to the Redux state.

### 10. Connect `logout` Action Creator to the Header

- **File:** `task_2/dashboard/src/Header/Header.js`
- **Description:** Connect `logout` action creator and user state to the `Header` component.

### 11. Modify the `uiReducer`

- **File:** `task_2/dashboard/src/reducers/uiReducer.js`
- **Description:** Update `uiReducer` to handle `LOGIN` and `LOGOUT` actions by setting and clearing user data.

### 12. Modify the Test Suites

- **Files:** `task_2/dashboard/src/App/App.test.js`, `task_2/dashboard/src/Footer/Footer.test.js`, `task_2/dashboard/src/Header/Header.test.js`, `task_2/dashboard/src/reducers/uiReducer.test.js`
- **Description:** Update test suites to reflect changes in the reducers and components.

### 13. Understand Redux DevTools Extension

- **File:** `task_3/dashboard/src/index.js`
- **Description:** Install Redux DevTools extension and configure it in your `index.js` file.

### 14. Combine Store: Root Reducer

- **File:** `task_4/dashboard/src/reducers/rootReducer.js`
- **Description:** Create and export a root reducer that combines `courseReducer`, `notificationReducer`, and `uiReducer`.

### 15. Combine Store: Modify the Application

- **File:** `task_4/dashboard/src/index.js`
- **Description:** Modify the store setup to use the root reducer.

### 16. Combine Store: Write the Tests

- **Files:** `task_4/dashboard/src/App/App.test.js`, `task_4/dashboard/src/reducers/rootReducer.test.js`
- **Description:** Update tests to work with the root reducer and combine reducers.

### 17. Connect Notifications: New Action Creator

- **File:** `task_5/dashboard/src/actions/notificationActionCreators.js`
- **Description:** Implement action creators for notifications including `setLoadingState`, `setNotifications`, and `fetchNotifications`.

### 18. Connect Notifications: Improve Reducer

- **File:** `task_5/dashboard/src/reducers/notificationReducer.js`
- **Description:** Update the `notificationReducer` to handle loading state and notifications data correctly.

### 19. Connect Notifications to the Reducer

- **File:** `task_5/dashboard/src/Notifications/Notifications.js`
- **Description:** Connect `Notifications` component to the Redux state and actions.

### 20. Connect Notifications: Clean Up

- **File:** `task_5/dashboard/src/App/App.js`
- **Description:** Remove obsolete functions and state related to notifications.

### 21. Connect Notifications: Update Test Suites

- **Files:** `task_5/dashboard/src/reducers/notificationReducer.test.js`, `task_5/dashboard/src/App/App.test.js`, `task_5/dashboard/src/Notifications/Notifications.test.js`, `task_5/dashboard/src/actions/notificationActionCreators.test.js`
- **Description:** Update tests to cover new notification actions and state changes.

### 22. Selectors

- **File:** `task_6/dashboard/src/selectors/notificationSelector.js`
- **Description:** Create memoized selectors for notifications using Redux Reselect.

### 23. Connect Courses: Create a Course Selector

- **File:** `task_7/dashboard/src/selectors/courseSelector.js`
- **Description:** Create a selector for fetching all course entities from the state.

### 24. Connect Courses: Create a Fetch Courses Function

- **File:** `task_7/dashboard/src/actions/courseActionCreators.js`
- **Description:** Implement `fetchCourses` action creator to fetch and dispatch course data.

### 25. Connect the Courses Component

- **File:** `task_7/dashboard/src/CourseList/CourseList.js`
- **Description:** Connect the `CourseList` component to Redux actions and selectors, and handle row changes.

### 26. Memoized Selectors: Redux Reselect

- **File:** `task_8/dashboard/src/selectors/notificationSelector.js`
- **Description:** Update selectors to use memoization with Redux Reselect.

### 27. Memoized Selectors: Update the UI

- **File:** `task_8/dashboard/src/Notifications/Notifications.js`
- **Description:** Update `Notifications` component to use memoized selectors and add filter buttons.

### 28. Memoized Selectors: Update the Test Suite

- **Files:** `task_8/dashboard/src/Notifications/Notifications.test.js`, `task_8/dashboard/src/selectors/notificationSelector.test.js`
- **Description:** Add tests for memoized selectors and update existing tests.

### 29. Container/Component

- **Files:** `task_9/dashboard/src/Notifications/Notifications.js`, `task_9/dashboard/src/Notifications/NotificationsContainer.js`
- **Description:** Refactor to use container components for connecting to Redux and fetching data.

