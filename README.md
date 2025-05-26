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
