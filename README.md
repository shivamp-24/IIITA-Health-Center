# IIITA Health Center Doctor Appointment Booking System

A full-stack web application built with the MERN stack to streamline doctor appointment scheduling. Students can log in, view doctor profiles, book and manage appointments, while admins can manage doctor information.

## Technologies Used

- **Frontend**: React, React Router, CSS
- **Backend**: Node.js, Express.js
- **Database**: MongoDB

### Day 1: Project Setup and Frontend Foundation

- **Project Initialization**:
  - Initialized a full-stack MERN project for a doctor appointment booking system.
  - Set up the development environment, including Node.js and React project initialization using `create-react-app` or equivalent.
  - Created a Git repository for version control and collaboration.
- **Frontend Folder Structure**:
  - Established a `Pages` folder in the frontend to organize React components for key pages (e.g., Homepage, Profile, Appointment Booking, Admin Dashboard).
  - Set up a modular folder structure to separate components, styles, and context logic.
- **Routing and Navigation**:
  - Configured React Router to define routes for different pages (e.g., `/`, `/profile`, `/appointments`).
  - Created and mounted a `Navbar` component for site-wide navigation, styled with CSS for `ul` and `hr` elements to ensure a clean and responsive design.
  - Defined navigation paths for seamless transitions between the homepage and other pages.
- **Authentication State Management**:
  - Implemented boolean state variables using React’s `useState` hook to manage user authentication status and enable conditional rendering of UI elements (e.g., showing login/logout options).
- **UI Components and Styling**:
  - Developed a `Header` component with a two-column layout (left and right sections) containing content and images, styled with CSS for responsiveness and smooth scrolling.
  - Added class names to `img` and `div` elements to ensure consistent styling across components.
  - Created a profile navigation section within the header for user profile access.
  - Built a specialty menu to display doctor profiles, styled with CSS to showcase details like name, specialty, and availability.
  - Designed a footer component with structured content and updated fonts for a cohesive UI.
  - Applied CSS properties to enhance the visual appeal of images, text, buttons, and layout sections (left, center, right).
- **Doctor Data Display and Filtering**:
  - Created UI components for rendering doctor data, including profile details and images.
  - Implemented filtering functionality to allow users to browse doctors by specialty, with dynamic CSS styling based on selected specialties.
  - Added navigation support for accessing doctor-specific pages and appointment booking interfaces.
- **Context for Shared Logic**:
  - Set up a React Context API to manage shared state and logic (e.g., authentication status, doctor data) across components.
  - Integrated context support in the frontend to streamline data flow and reduce prop drilling.

### Day 2: Frontend Page Development and Appointment Booking UI

- **New Page Creation**:
  - Developed the `Doctor Appointment` page in the `Pages` folder to display doctor details, booking slots, and related doctors.
  - Created `About` and `Contact` pages to provide information about the platform and contact options.
  - Built a `Login` page with a form for user authentication.
  - Designed a `Patient Profile` page to display and edit user details, including profile picture functionality.
- **Doctor Appointment Page**:
  - Displayed doctor data (e.g., name, specialty, experience) and images using props for dynamic rendering.
  - Implemented a related doctors section with filtering by specialty, leveraging `useEffect` hook and props for dynamic updates.
  - Added a booking slot interface:
    - Created state variables with `useState` to store and manage available appointment slots.
    - Set up date and time selection for booking, including logic to calculate available slots.
    - Fixed date format errors to ensure correct display.
    - Displayed selected date’s time slots with dynamic class names and `onClick` event handlers for user interaction.
    - Customized currency symbols for pricing details in the booking interface.
  - Applied CSS properties to style booking slots, doctor profiles, and related sections for a cohesive and responsive layout.
- **About and Contact Pages**:
  - Structured sections with `div` elements, uppercase text, images, and buttons for improved user experience.
  - Applied CSS properties to enhance layout, typography, and visual appeal of section elements.
- **Login Page**:
  - Initialized state for form inputs using `useState` to handle dynamic text updates.
  - Created a login form with styled input fields, implementing logic for account creation and login state management.
  - Applied CSS properties to design a responsive and user-friendly form layout.
- **Patient Profile Page**:
  - Built a user details object to store profile information (e.g., address, gender, basic details).
  - Implemented editing functionality with conditional rendering to update profile fields.
  - Added input fields for gender selection and date, styled with CSS for consistency.
  - Designed UI for profile picture editing, allowing users to upload or update images.
  - Applied CSS properties to format the profile page layout for a polished appearance.
- **UI and Styling Enhancements**:
  - Added dynamic styling for sections using CSS, including layout divisions (left, center, right) and uppercase text for headings.
  - Improved overall design with consistent typography, spacing, and responsive layouts across all new pages.
  - Ensured smooth navigation and interactivity with `onClick` events and dynamic class names for doctor filtering and booking slots.

### Day 3: Backend Setup, Database Integration, and Responsive UI

- **Dependency Installation**:
  - Installed backend dependencies: `express`, `mongoose`, `multer`, `bcrypt`, `cloudinary`, `cors`, `dotenv`, `jsonwebtoken`, `nodemon`, and `validator` to enable server setup, database management, file uploads, authentication, and input validation.
- **Appointments Page Development**:
  - Created an `Appointments` page in the `Pages` folder to display doctor data, including profiles, booking slots, and related information.
  - Styled the page with CSS to present doctor details (e.g., name, specialty, experience) in a user-friendly format.
- **Responsive Design Enhancements**:
  - Made the website responsive by applying CSS properties to ensure compatibility across devices.
  - Developed a mobile menu with styled `ul` and `li` elements, including a filter button to toggle menu display.
  - Added CSS for menu links and section elements to enhance mobile usability and visual appeal.
- **Backend Server Setup**:
  - Initialized an Express.js server using `express` to handle API requests.
  - Created a server script with `nodemon` for automatic restarts during development.
  - Configured `cors` to enable communication between the React frontend and Express backend.
  - Set up environment variables using `dotenv` to securely store sensitive data (e.g., MongoDB Atlas URL, Cloudinary credentials) in a `.env` file.
- **MongoDB Atlas Integration**:
  - Established a connection to MongoDB Atlas using `mongoose`, configuring the database URL via environment variables.
  - Created a database user and set up the connection string for secure access.
- **Data Models**:
  - Defined a `Doctor` model with a schema in `mongoose` to store doctor data (e.g., name, specialty, experience, image).
  - Created a `User` model to store patient and admin data, including fields for authentication (e.g., email, hashed password).
- **API and Admin Functionality**:
  - Developed controller functions for APIs to manage doctor data, including an endpoint to add doctor data to the database.
  - Created an admin router and endpoint for managing doctor information via an admin panel.
  - Implemented `multer` middleware with `cloudinary` for uploading doctor profile images, storing URLs in the database.
  - Added form fields for the doctor appointment booking form, with validation using `validator` for input checking (e.g., email format, required fields).
- **Authentication and Security**:
  - Used `bcrypt` to hash and securely store passwords for user accounts (e.g., admin and patient logins).
  - Implemented admin login functionality with `jsonwebtoken` to generate tokens based on email and password validation.
  - Created authentication middleware to verify tokens and protect admin routes, ensuring secure access to the admin panel.
  - Resolved validation errors and configured assets (e.g., uploaded images) for proper storage and retrieval.

### Day 4: Admin Panel Development and Doctor Management

- **Dependency Installation**:
  - Installed frontend dependencies: `axios` for API requests, `react-router-dom` for admin panel routing, and `react-toastify` for user feedback notifications.
  - Installed dev dependencies: `tailwindcss`, `postcss`, and `autoprefixer` for styling the admin panel.
  - Initialized Tailwind CSS with `npx tailwindcss init -p` to set up configuration files.
- **Admin Panel Setup**:
  - Created an admin panel section in the frontend to manage doctor data and system operations.
  - Configured the project to run on specific ports, ensuring separation of frontend and backend services.
  - Set up admin-specific assets (e.g., images, styles) and a React Context for managing admin-related state and logic.
  - Established context providers for different user roles (e.g., admin, doctor) to handle role-specific functionality.
- **Admin Authentication**:
  - Developed state variables with `useState` to manage admin and doctor login states.
  - Created a login form with email and password input fields, marked as `required`, styled with Tailwind CSS.
  - Implemented admin login functionality:
    - Created a form submission function to make API calls using `axios` based on user state.
    - Fetched and stored authentication tokens from the backend for secure admin access.
    - Added middleware to manage admin access with token storage and verification.
    - Implemented logout functionality with a dedicated button in the admin panel.
- **Admin Dashboard UI**:
  - Designed the admin dashboard UI with a sidebar for navigation, styled using Tailwind CSS.
  - Added menu items to the sidebar with icons and text, using dynamic class names for active navigation links.
  - Styled dashboard elements (e.g., text, logo, logout button) with Tailwind CSS for a responsive and modern look.
  - Configured routes with `react-router-dom` for seamless navigation within the admin panel (e.g., dashboard, add doctor page).
- **Add Doctor Functionality**:
  - Created an `Add Doctor` page with a form including input fields for doctor details (e.g., name, experience, fee) and a `select` tag for options like experience level.
  - Linked form inputs to state variables using `useState` for real-time updates.
  - Integrated `multer` and `cloudinary` (from Day 3) to handle doctor image uploads, displaying selected images in the form.
  - Connected form submission to an API call using `axios` to add doctor data to the MongoDB database.
  - Used `react-toastify` to display success or error messages after form submission.
  - Reset input fields and image tags after successful submission for a clean user experience.
- **Doctor Data Management**:
  - Added 15 sample doctors to the MongoDB database via an API endpoint.
  - Created an API to fetch all doctor data for display in the admin panel.
  - Developed a UI section in the admin panel to list all doctors, retrieving details (e.g., name, specialty) with `axios` requests.
  - Styled the doctor list with Tailwind CSS for clarity and responsiveness.
- **Additional Enhancements**:
  - Logged form values using template literals for debugging and validation.
  - Resolved validation errors during form submission to ensure data integrity.

### Day 5: Doctor Data Display, Patient Authentication, and Profile Management

- **Doctor Data Display**:
  - Created an API call using `axios` to fetch all doctor data from the MongoDB database for display in the admin panel and frontend website.
  - Developed UI elements on the frontend to render the doctor list, including details like name, specialty, and availability.
  - Applied Tailwind CSS (from Day 4) to style the doctor appointment booking page for a responsive and visually appealing layout.
  - Implemented functionality to update doctor availability:
    - Created a route and controller function to toggle availability status in the database.
    - Updated the frontend to reflect changes in real-time using `axios` API calls.
  - Defined a function to retrieve and display the doctor list on the frontend, ensuring seamless integration with the backend.
- **Patient Login and Registration System**:
  - Developed API logic for user authentication and appointment booking:
    - Created a user registration route, saving user data (e.g., name, email, password) to MongoDB with `bcrypt` for password hashing.
    - Implemented `jsonwebtoken` (JWT) to generate authentication tokens upon registration and login.
    - Added validation for name, email, and password fields using `validator` to ensure data integrity.
    - Handled registration errors (e.g., duplicate emails) with `try-catch` blocks and displayed feedback using `react-toastify`.
  - Built a user login function:
    - Created a login route to authenticate users by verifying email and password with `bcrypt`.
    - Stored JWT tokens in React Context for persistent authentication across the frontend.
    - Integrated login and registration forms with the frontend, linking form inputs to API calls via `axios`.
  - Set up environment variables in the frontend (e.g., API base URL) using `dotenv` for secure configuration.
  - Configured `react-toastify` to display error notifications for failed login or registration attempts.
- **Patient Profile Management**:
  - Created an API to retrieve and update patient profile data, including fields like name, email, address, and profile image.
  - Developed a controller function to handle profile updates, checking available properties before saving changes to MongoDB.
  - Implemented image upload functionality for patient profiles using `multer` and `cloudinary`, storing image URLs in the database.
  - Built middleware functions for user authentication:
    - Created authentication middleware to verify JWT tokens for protected profile routes.
    - Added multiple middleware checks to ensure secure data updates.
  - Enhanced the patient profile page UI with Tailwind CSS for styling form inputs, image displays, and layout sections.
  - Used `try-catch` blocks in arrow functions to handle errors during profile updates, ensuring robust error handling.
