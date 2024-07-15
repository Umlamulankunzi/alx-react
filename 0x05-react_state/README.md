# React State Management Project

## Learning Objectives

By the end of this project, you should be able to explain:

- What the state of a component or a container is.
- The lifecycle of a component.
- How to modify a state and execute code in the right order.
- What a controlled component is.
- How to use Forms in React.
- How to reuse smaller components, keep them pure, and lift their state to principal containers.
- The use of a React Hook and how to create one.
- How to test State changes with Enzyme.

## Requirements

- All your files will be interpreted/compiled on Ubuntu 18.04 LTS using Node.js 12.x.x and npm 6.x.x.
- Allowed editors: vi, vim, emacs, Visual Studio Code.
- All your files should end with a new line.
- A `README.md` file, at the root of the folder of the project, is mandatory.

## Tasks

### 0. Adding a Local State for Notifications

- **File modifications:**
  - `task_0/dashboard/src/App/App.js`
  - `task_0/dashboard/src/App/App.test.js`
  - `task_0/dashboard/src/Notifications/Notifications.js`
  - `task_0/dashboard/src/Notifications/Notifications.test.js`

- **Steps:**
  - Create a local state for `displayDrawer`.
  - Define default state in the constructor.
  - Create `handleDisplayDrawer` and `handleHideDrawer` functions.
  - Pass `displayDrawer`, `handleDisplayDrawer`, and `handleHideDrawer` as props to `Notifications`.
  - Add tests to verify state changes in `App.test.js` and `Notifications.test.js`.

### 1. Controlled Components and State Callback

- **File modifications:**
  - `task_1/dashboard/src/Login/Login.js`
  - `task_1/dashboard/src/Login/Login.test.js`

- **Steps:**
  - Create a form in `Login` and handle submit.
  - Add state values for `email` and `password`.
  - Create `handleChangeEmail` and `handleChangePassword` functions.
  - Add `enableSubmit` state and logic to enable/disable the submit button.
  - Add tests for form behavior and state updates.

### 2. Context

- **File modifications:**
  - `task_2/dashboard/src/App/AppContext.js`
  - `task_2/dashboard/src/App/App.js`
  - `task_2/dashboard/src/Login/Login.js`
  - `task_2/dashboard/src/Header/Header.js`
  - `task_2/dashboard/src/Header/Header.test.js`
  - `task_2/dashboard/src/App/App.test.js`

- **Steps:**
  - Create a React context for user state and logOut function.
  - Modify `App` to use context for state and pass `logIn` function.
  - Update `Header` to display user info and handle logOut.
  - Add tests to verify context usage and state updates.

### 3. Context Consumer & Advanced State

- **File modifications:**
  - `task_3/dashboard/src/Footer/Footer.js`
  - `task_3/dashboard/src/Footer/Footer.test.js`
  - `task_3/dashboard/src/App/App.js`
  - `task_3/dashboard/src/App/App.test.js`
  - `task_3/dashboard/src/Notifications/Notifications.js`
  - `task_3/dashboard/src/Notifications/Notifications.test.js`

- **Steps:**
  - Modify `Footer` to subscribe to context changes.
  - Add `markNotificationAsRead` function in `App` and pass it to `Notifications`.
  - Refactor `Notifications` to use the new function.
  - Add tests to verify context behavior and state updates.

### 4. Introduction to React Hook

- **File modifications:**
  - `task_4/dashboard/src/CourseList/CourseListRow.js`

- **Steps:**
  - Use React Hooks to manage state in `CourseListRow`.
  - Add a checkbox to simple rows and update the row style when checked.

## Tips & Requirements

- Use `setState` and instance methods when creating tests with Enzyme.
- Bind functions passed to children for performance improvements.
- Ensure no lint errors in the console.
- Remember that function components cannot use the context directly; consider converting to classes if necessary.
- Do not forget to export elements that are reused throughout the app.
- Clean unused state and props after refactoring.
- Set `propTypes` and `defaultProps` for any new props.

## Repository

- **GitHub repository:** `alx-react`
- **Main directory:** `0x05-react_state`

### Files by Task

- **Task 0:** `task_0/dashboard/src/App/App.js`, `task_0/dashboard/src/App/App.test.js`, `task_0/dashboard/src/Notifications/Notifications.js`, `task_0/dashboard/src/Notifications/Notifications.test.js`
- **Task 1:** `task_1/dashboard/src/Login/Login.js`, `task_1/dashboard/src/Login/Login.test.js`
- **Task 2:** `task_2/dashboard/src/App/AppContext.js`, `task_2/dashboard/src/App/App.js`, `task_2/dashboard/src/Login/Login.js`, `task_2/dashboard/src/Header/Header.js`, `task_2/dashboard/src/Header/Header.test.js`, `task_2/dashboard/src/App/App.test.js`
- **Task 3:** `task_3/dashboard/src/Footer/Footer.js`, `task_3/dashboard/src/Footer/Footer.test.js`, `task_3/dashboard/src/App/App.js`, `task_3/dashboard/src/App/App.test.js`, `task_3/dashboard/src/Notifications/Notifications.js`, `task_3/dashboard/src/Notifications/Notifications.test.js`
- **Task 4:** `task_4/dashboard/src/CourseList/CourseListRow.js`