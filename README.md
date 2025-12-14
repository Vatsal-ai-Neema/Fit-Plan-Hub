# Fit-Plan-Hub 

Project Overview
FitPlanHub Pro is a modern, responsive web application designed to connect Fitness Trainers with Users. This frontend repository represents the "Pro" interface, featuring a polished UI, real-time interactions, and a simulated state-management system.

It follows a "Frontend-First" workflow, allowing for rapid UI testing and logic validation using mock data before backend integration.

 Key Features
 UI/UX Design
Modern Theming: Uses CSS Variables (:root) for consistent color palettes (Dark Mode compatible).

Glassmorphism & Grids: specialized card layouts using CSS Grid and Flexbox.

Visual Feedback: Hover states, transitions, and "Toast" notifications (custom popups) instead of native browser alerts.

Responsive: Adapts from Desktop to Mobile views seamlessly.

 Functional Logic
Role-Based Access Control (RBAC):

Trainers: Can create and publish new plans via a specialized dashboard.

Users: Can browse, filter, and subscribe to plans.

Smart Search & Filtering: Real-time filtering by Category (Cardio, Strength, Yoga) and Search keywords.

Subscription Constraints: Logic to prevent users from subscribing to multiple active plans simultaneously.

Content Locking: CSS filter: blur() applied to premium content until a valid subscription state is detected.

🛠️ Tech Stack
Component,Technology,Description
Structure,HTML5,"Semantic tags (<nav>, <section>, <article>)"
Styling,CSS3,"CSS Variables, Flexbox, Grid, Keyframe Animations"
Logic,Vanilla JS (ES6+),"Arrow functions, Template Literals, DOM Manipulation"
Assets,Unsplash API,Remote image fetching for realistic prototypes
Fonts,Google Fonts,'Poppins' for modern typography

⚡ Setup & Run Instructions
Since this project uses a Monolithic Frontend Architecture, no build tools (Webpack/Vite) or package managers (NPM) are required for the view layer.

Download: Ensure index.html is in your project folder.

Run: Double-click index.html to open it in Chrome, Edge, or Safari.

Test Credentials:
User Mode: Enter any name, select "User".

Trainer Mode: Enter any name, select "Trainer".

🔮 Future Roadmap (Backend Integration)
To move this from "Prototype" to "Production", the following developer workflow changes are planned:

[ ] Decouple Files: Separate into style.css, script.js, and index.html.

[ ] API Connection: Replace plans array with fetch('http://localhost:3000/api/plans').

[ ] Auth: Replace local variable currentUser with JWT (JSON Web Tokens) stored in LocalStorage.

[ ] Database: Connect Mongoose/MongoDB to persist plans permanently.
