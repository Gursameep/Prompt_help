*Important Prompts used*

**Prompt 1: To build Portfolio webpage in HTML, CSS, JS**

I want you to create an responsive portfolio for myself, Built is as a Senior Frontend Developer, Responsive Portfolio Checklist Core Layout and Design
Fluid Grid Layout: Use Flexbox or Grid so elements rearrange based on screen size.
Mobile-First Navigation: A hamburger menu for mobile that expands into a full bar for desktop.
Scalable Typography: Use relative units like rem or em for font sizes to ensure readability.
Large Tap Targets: Ensure buttons and links are easy to click with a thumb on mobile. Media and Performance
Responsive Images: Use srcset to serve appropriately sized images to different devices.
Lazy Loading: Set images to load only as they enter the viewport to save bandwidth.
SVG Graphics: Use vectors for logos and icons to maintain sharpness at any size.
Performance Optimization: Aim for fast load times to prevent high bounce rates. Content and Sections
Sticky Header: Keep navigation accessible at all times during a scroll.
Hero Statement: A clear "above-the-fold" summary of your identity and skills.
Scannable Projects: Vertical stacks for mobile and multi-column grids for desktop.
One-Tap Contact: Hyperlinked email and phone numbers for immediate outreach. Technical Requirements
Cross-Browser Support: Consistent functionality across Chrome, Safari, and Firefox.
Form Usability: Prevent mobile browsers from auto-zooming on text input fields.

**Prompt 2: To build Auth APIs for Login/Signup/Logout**
Build a complete backend REST API for user authentication with the following requirements:
Tech Stack:
- Node.js
- Express.js
- MongoDB with Mongoose
- JWT (JSON Web Token) for authentication
- bcrypt for password hashing
- Zod for request validation
- Swagger (OpenAPI) for API documentation

Features:
- User Signup
- User Login
- User Logout (JWT invalidation or client-side handling explanation)

Project Structure:
Follow MVC architecture with this folder structure:
- /config (database connection, swagger config)
- /models (User model using Mongoose)
- /controllers (auth controller: signup, login, logout)
- /routes (auth routes)
- /middlewares (auth middleware, error handling, validation)
- /validators (Zod schemas for signup and login)
- /utils (JWT helpers, response helpers if needed)
- server.js (entry point)

Functional Requirements:
1. Signup:
   - Validate request body using Zod
   - Hash password using bcrypt
   - Store user in MongoDB
   - Return success response with JWT

2. Login:
   - Validate request body using Zod
   - Check user existence
   - Compare password using bcrypt
   - Return JWT token

3. Logout:
   - Implement basic logout (client-side token removal)
   - Optionally explain token blacklist strategy

4. JWT:
   - Use middleware to protect routes
   - Store secret in environment variables

5. Swagger:
   - Document all APIs (/signup, /login, /logout)
   - Provide Swagger UI setup at /api-docs

6. Error Handling:
   - Centralized error handler middleware
   - Proper HTTP status codes and messages

7. Database:
   - Mongoose User schema with fields:
     - name
     - email (unique)
     - password

8. Testing:
   - Provide sample API test cases using:
     - Postman collection OR
     - curl commands
   - Include example request/response bodies

9. server.js:
   - Setup express app
   - Connect MongoDB
   - Register routes
   - Setup middleware
   - Start server

10. Environment Variables:
   - PORT
   - MONGO_URI
   - JWT_SECRET

Extras:
- Use async/await
- Clean and readable code
- Add comments for clarity

Output:
- Provide full working code for all files
- Include instructions to run the project
- Include sample .env file
 
**Prompt 3: To build Portfolio webpage using React JS, Tailwind CSS**

Build a fully responsive personal portfolio website using React.js and Tailwind CSS, following modern frontend architecture and best practices expected from a Senior Frontend Developer.
Tech Stack
React.js (with functional components and hooks)
Tailwind CSS for styling
Optional: React Router (if multi-page)
Optional: Framer Motion (for animations)

Core Layout and Design
Responsive Layout
Use Flexbox and CSS Grid (via Tailwind utilities) to create a fluid, adaptive layout.
Follow a mobile-first approach and progressively enhance for tablets and desktops.
Use Tailwind breakpoints (sm, md, lg, xl) effectively.
Navigation
Implement a responsive navbar:
Mobile: hamburger menu with slide-in or dropdown behavior
Desktop: full horizontal navigation bar
Add smooth scrolling to sections.
Typography
Use relative units (rem, em) for scalability.
Maintain clear visual hierarchy using Tailwind typography utilities.
Accessibility & UX
Ensure large tap targets (min 44px height/width).
Use semantic HTML and ARIA attributes where necessary.
Maintain proper color contrast.

Media and Performance
Images
Use responsive images (<img srcSet /> or modern React image handling).
Implement lazy loading using loading="lazy" or intersection observer.
Graphics
Use SVGs for icons and logos (via inline SVG or libraries like Heroicons).
Performance Optimization
Code splitting (React lazy/Suspense if needed)
Optimize images and assets
Minimize re-renders using memoization where appropriate

Content Sections
1. Sticky Header
Fixed or sticky navbar always visible during scroll.
2. Hero Section
Clear headline introducing:
Name
Role (Senior Frontend Developer)
Short value proposition
CTA buttons (e.g., “View Projects”, “Contact Me”)
3. About Section
Brief professional summary
Skills and technologies (React, Tailwind, etc.)
4. Projects Section
Responsive layout:
Mobile: vertical stacked cards
Desktop: grid layout (2–3 columns)
Each project card includes:
Title
Description
Tech stack
Live demo + GitHub links
5. Contact Section
Contact form with validation
One-tap actions:
Clickable email (mailto:)
Clickable phone (tel:)

Technical Requirements
Form Handling
Prevent mobile auto-zoom on inputs (font-size ≥ 16px)
Validate inputs (basic validation or using a library like React Hook Form)
Cross-Browser Compatibility
Ensure consistent behavior across:
Chrome
Safari
Firefox
State Management
Use React hooks (useState, useEffect)
Keep components modular and reusable

Project Structure
/src
/components
Navbar.jsx
Hero.jsx
About.jsx
Projects.jsx
Contact.jsx
Footer.jsx
/assets
/data (project data, constants)
App.jsx
main.jsx

Styling Guidelines
Use Tailwind utility classes (avoid custom CSS unless necessary)
Maintain consistent spacing using Tailwind spacing scale
Use a clean, modern design aesthetic

Extras (Optional but Recommended)
Dark mode toggle
Smooth animations (Framer Motion)
Scroll reveal effects
SEO meta tags

Output Requirements
Provide full working React code
Include Tailwind setup instructions
Ensure code is clean, modular, and well-commented
Include instructions to run the project (npm install, npm run dev/build)

