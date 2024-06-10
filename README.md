# job-management-dashboard

The Job Management System is a full-stack web application designed to streamline job listing, management, and tracking processes. It consists of both frontend application that provides a user-friendly interface and backend API application for handling data storage, retrieval and manipulation operations.

## Getting Started

Follow the instructions below to set up and run the frontend application locally:

### Starting the backend application

1. On any directory on your machine, clone this repository.
2. Navigate to the `job_management_backend` directory using the command: `cd job-management-dashboard/job_management_backend`
3. Install dependencies: `npm install`.
4. Start the backend server: `node server.js`.

### Starting the frontend application
1. On another terminal, navigate to the `job-management-frontend` directory using the command: `cd job-management-dashboard/job-management-frontend`
2. Install dependencies: `npm install`.
3. Start the development server: `npm start`.
4. Open your browser and visit `http://localhost:3000` to view the application.

# Backend Application Details

This is the backend application for the job management system. It serves as the server-side component responsible for handling data storage, retrieval, and manipulation operations.

## Features

- **Job Data Management:** Storing and managing job data in a JSON file stored on the backend.
- **RESTful API:** Exposing RESTful API endpoints to perform CRUD operations on job data.
- **Request Handling:** Handling HTTP requests from the frontend application and processing them accordingly.
- **Error Handling:** Handling errors gracefully and providing appropriate error responses.

## Architecture
The backend is built using Node.js with the Express.js framework. It follows a RESTful architecture for managing job data. The architecture is modular, separating concerns like routes,utility files from the entry point file.

## Technologies Used

- Node.js: JavaScript runtime for building server-side applications.
- Express.js: Web application framework for Node.js for handling HTTP requests.
- fs: A Node.js module for interacting with the file system, allowing oopeartions such as reading and writing. As a JSON file was used to as the databse, fs module was used to interact with the file.
- cors: Middleware for enabling Cross-Origin Resource Sharing.

## API Documentation
- GET /jobs: Retrieve a list of all jobs.
- GET /jobs/:id: Retrieve a specific job by its ID.
- POST /jobs: Create a new job.
- PUT /jobs/:id: Update an existing job by its ID.
- DELETE /jobs/:id: Delete an existing job by its ID.

# Frontend Application Details

This is the frontend application for the job management system. It provides a user-friendly interface for interacting with the backend API to perform various job-related actions.

## Features

- **Listing All Jobs:** Displaying a list of all available jobs on landing page.
- **Viewing Job Details:** Viewing detailed information about a specific job in a popup once the View button is clicked.
- **Posting New Job:** Allowing users to create and post new job listings.
- **Updating Existing Job:** Providing functionality to update details of existing job listings once the Ediyt button is clicked.
- **Deleting Existing Job:** Allowing users to delete job listings once the Delete button is clicked.
- **Form Validation:** Ensuring data integrity through form validation. All fields are required.
- **Client-Side Routing:** Providing a seamless navigation experience within the application.

## Technologies Used

- React.js: JavaScript library for building user interfaces.
- react-router-dom: Client-side routing for navigating between pages.
- fetch function: For making HTTP requests to the backend API.
- formik: Form management library for building and validating forms.
- reactstrap and bootstrap: Bootstrap is a frontend framework for quickly spinning up responsive and modern websites. Reactstrap is a React components library based on Bootstrap for UI components. A combination of these 2 libraries were used for the site design.