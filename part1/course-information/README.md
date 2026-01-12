# Course Information

A React application developed as part of the Full Stack Open curriculum. The project focuses on the core principles of component-based architecture and unidirectional data flow.

## Project Overview

The application displays details about a specific development course, including the course name, various modules (parts), and the total count of exercises. The project evolved from simple variables into a single, complex JavaScript object passed through nested components.

## Technical Implementations

The final version of this project (Step 5) implements the following:

### 1. Component Architecture

* **Header**: Renders the course name.
* **Content**: Orchestrates the rendering of specific course parts.
* **Part**: A reusable component for individual module details.
* **Footer**: Calculates and displays the aggregate number of exercises.

### 2. Data Structure

The application utilizes a nested data model to manage information:

* **Object-Oriented**: Data is encapsulated within a single `course` object.
* **Arrays**: Course modules are stored in an array of objects to facilitate future scalability.

### 3. Props Management

* **Prop Drilling**: Demonstrates passing data from the root `App` component down to deeply nested `Part` components.
* **Object Destructuring**: Accessing nested properties via dot notation (e.g., `props.course.parts[0].exercises`).

## Getting Started

### Prerequisites

* Node.js (LTS version recommended)
* npm or yarn

### Installation

1. Clone the repository or navigate to the project folder.
2. Install the necessary dependencies:
```bash
npm install

```



### Development

To run the application in development mode with Hot Module Replacement (HMR):

```bash
npm run dev

```

The application will be accessible at `http://localhost:5173` by default.

## Progress Summary

* **Exercises 1.1 - 1.2**: Established component nesting.
* **Exercises 1.3 - 1.4**: Transitioned from individual variables to arrays of objects.
* **Exercise 1.5**: Refactored the entire state into a single unified object.
