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
