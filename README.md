# Solvei8 Authentication Module

This project is an authentication module built with Angular, providing a user-friendly interface for creating accounts and logging in. The module includes form validation, progress indicators, and success screens to enhance the user experience.

## Table of Contents
- [Project Structure](#project-structure)
- [Prerequisites](#prerequisites)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [Components](#components)
- [Routes](#routes)
- [Development](#development)
- [License](#license)

## Project Structure
```
src/
│
├── app/
│   ├── auth/
│   │   ├── login/
│   │   │   ├── login.component.html
│   │   │   ├── login.component.scss
│   │   │   ├── login.component.ts
│   │   ├── sign-up/
│   │   │   ├── sign-up.component.html
│   │   │   ├── sign-up.component.scss
│   │   │   ├── sign-up.component.ts
│   ├── app.module.ts
│   ├── app.component.ts
│   ├── app.component.html
│   ├── app.component.scss
│   ├── app-routing.module.ts
├── assets/
│   ├── images/
│   ├── styles/
└── index.html
```

## Prerequisites

- **Node.js**: Ensure you have Node.js installed. You can download it from [Node.js official website](https://nodejs.org/).
- **Angular CLI**: Install Angular CLI globally by running the following command:
  ```bash
  npm install -g @angular/cli
  ```

## Setup Instructions

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/solvei8-auth-module.git
   cd solvei8-auth-module
   ```

2. **Install Dependencies:**
   Install the necessary dependencies by running:
   ```bash
   npm install
   ```

3. **Serve the Application:**
   Start the development server by running:
   ```bash
   ng serve
   ```
   The application will be available at `http://localhost:4200/`.

## Usage

### Sign Up
- The sign-up form consists of two steps:
  1. **Step 1**: Collects user email, full name, and password.
  2. **Step 2**: Collects organization details such as name, ID, designation, date of birth, city, and pincode.

- The progress indicator at the top shows the current step. The user can navigate back to the previous step using the "Go Back" button.

### Login
- The login form allows users to enter their email and password to access their account.
- If the login is successful, a success screen is displayed, and the user is redirected to the dashboard.

### Thank You Page
- After successful registration, a thank you page is displayed, and the user is automatically redirected to the login page.

## Components

### LoginComponent
- **Location**: `src/app/auth/login/login.component.ts`
- **Description**: Handles user login functionality.

### SignUpComponent
- **Location**: `src/app/auth/sign-up/sign-up.component.ts`
- **Description**: Manages the user sign-up process, including form validation and multi-step navigation.

## Routes

The following routes are defined in the application:

- **`/login`**: Renders the `LoginComponent`.
- **`/signup`**: Renders the `SignUpComponent`.
- **`**`**: Redirects to the `/login` route by default.

## Development

To modify or extend the application:

1. **Create Components**: Use Angular CLI to generate new components:
   ```bash
   ng generate component component-name
   ```

2. **Update Routes**: Modify `src/app/app-routing.module.ts` to add or update routes.

3. **Styling**: Tailwind CSS is used for styling. Customize styles in the respective component SCSS files.
