# CS 290 - Web Development

Complete collection of web development assignments covering front-end technologies (HTML, CSS, JavaScript), DOM manipulation, database integration, and full-stack MERN application development with Node.js, Express, React, and MongoDB.

## Course Overview

Comprehensive introduction to modern full-stack web development, progressing from fundamental front-end technologies through advanced back-end API development and database integration, culminating in a complete MERN stack application.

---

## Assignments Overview

### Assignment 1: HTTP Basics & Browser DevTools
**Files:** `campmeli-a1.pdf` (submission proof)  
**Topics:** HTTP requests (GET/POST), browser developer tools, network inspection  
**Description:** Introduction to HTTP fundamentals, examining request/response cycles, URL parameters, network headers, status codes (200, 404), and browser console usage.  
**Skills:** Understanding HTTP protocol, using browser DevTools, debugging web requests

---

### Assignment 2: HTML & CSS Fundamentals
**Files:** `index.html`, `contact.html`, `global.css`  
**Topics:** HTML structure, CSS styling, responsive design  
**Description:** Built a two-page "Beaver Store" website with proper HTML semantic structure and CSS styling. Created navigation between pages, implemented HTML tables, forms, and applied the CSS box model for layout and design.

**Features:**
- Semantic HTML5 structure (`<header>`, `<nav>`, `<main>`, `<footer>`)
- CSS styling with custom fonts, colors, backgrounds, borders
- HTML tables for product listings
- Navigation links between pages
- Contact information using definition lists
- Responsive layout with flexbox

**Concepts:** HTML5 semantics, CSS selectors, box model, typography, color theory, page layout

---

### Assignment 3: JavaScript Fundamentals
**File:** `deepEqual.js`  
**Topics:** JavaScript data types, objects, arrays, loops, conditionals, recursion  
**Description:** Implemented a `deepEqual` function that performs deep equality comparison between two JavaScript values, handling primitives, objects, and arrays with recursive logic.

**Features:**
- Handles all JavaScript primitive types (numbers, booleans, strings, null, undefined)
- Deep comparison of objects and arrays
- Recursive algorithm for nested structures
- Comprehensive unit test suite (Jest)

**Concepts:** Type checking, recursion, object property iteration, array comparison, test-driven development

---

### Assignment 4: Advanced JavaScript
**Files:** `reducers.mjs`, `Point2D.mjs`, `Point3D.mjs`  
**Topics:** Higher-order functions, object-oriented programming, ES6 classes, exceptions  
**Description:** Two-part assignment demonstrating functional programming and OOP principles in JavaScript.

**Part 1: Reducer Functions**
- `reducer1` - Sums numeric array values, skipping non-numeric elements
- `reducer2` - Sums array values or throws TypeError for non-numeric elements
- Demonstrates functional programming with `Array.reduce()`

**Part 2: Point Classes**
- `Point2D` - Class modeling 2D points with Euclidean distance calculation
- `Point3D` - Extends Point2D for 3D space
- Demonstrates class inheritance and method overriding

**Concepts:** Higher-order functions, ES6 classes, inheritance, exceptions, ES modules (import/export), mathematical computations

---

### Assignment 5: DOM Manipulation & Interactive Web Pages
**Files:** `order.html`, `tableWriter.js`, `orderProcessor.js`  
**Topics:** Document Object Model (DOM), events, form handling, dynamic content  
**Description:** Created interactive web pages using JavaScript to dynamically manipulate the DOM and respond to user events.

**Features:**
- Dynamically generated HTML tables from JavaScript data
- Form validation and submission handling
- Event listeners for user interactions
- Dynamic row addition to tables
- DOM element creation and manipulation

**Concepts:** DOM tree traversal, `document` methods, event handling, form data extraction, preventing default behaviors, dynamic HTML generation

---

### Assignment 6: REST API with Node.js & Express
**Files:** `model.mjs`, `controller.mjs`  
**Topics:** REST APIs, HTTP methods, Node.js, Express framework, MVC pattern  
**Description:** Built a complete REST API for managing stock orders using Node.js and Express, implementing full CRUD operations following REST principles.

**API Endpoints:**
- `POST /orders` - Create new order (201 Created)
- `GET /orders` - Retrieve all orders with optional company filter
- `GET /orders/:id` - Retrieve specific order (200 OK / 404 Not Found)
- `PUT /orders/:id` - Update order quantity (200 OK / 400 Bad Request / 404 Not Found)
- `DELETE /orders/:id` - Delete order (204 No Content / 404 Not Found)

**Features:**
- RESTful API design
- Input validation
- Proper HTTP status codes and headers
- JSON request/response handling
- MVC architecture (Model-View-Controller)
- Error handling

**Concepts:** REST principles, HTTP methods (GET, POST, PUT, DELETE), status codes, Express routing, middleware, request/response handling, MVC pattern, API testing

---

### Assignment 7: Database Persistence with MongoDB
**Files:** `users_model.mjs`, `users_controller.mjs`  
**Topics:** MongoDB, Mongoose ODM, asynchronous JavaScript, database operations  
**Description:** Built a REST API for user management with MongoDB database persistence using Mongoose for data modeling and validation.

**Data Model:**
- **User Properties:** name (String), age (Number), email (String), phoneNumber (Number, optional), _id (auto-generated)
- Phone number validation: integers only, no spaces/hyphens, cannot start with 0

**API Endpoints:**
- `POST /users` - Create user (201 / 400)
- `GET /users` - Retrieve all users (200)
- `GET /users/:id` - Retrieve user by ID (200 / 404)
- `PUT /users/:id` - Update user (200 / 400 / 404)
- `DELETE /users/:id` - Delete user (204 / 404)

**Features:**
- MongoDB integration with Mongoose ODM
- Schema validation and data modeling
- Asynchronous operations with async/await
- Environment variables for database configuration
- Input validation and error handling

**Concepts:** NoSQL databases, MongoDB, Mongoose schemas, async/await, promises, database CRUD operations, data validation, connection management

---

### Assignment 8: React Single Page Application
**Files:** React components (.jsx), CSS styling  
**Topics:** React framework, JSX, State Hook, React Router, Single Page Applications  
**Description:** Developed a client-side Single Page Application (SPA) using React with routing between multiple pages. Uses canned data (no backend).

**Pages:**
- Homepage - Product display
- Order Page - Order form
- Registration Page - User registration

**Features:**
- Function-based React components
- React Router for navigation
- State management with useState Hook
- Form handling in React
- Navigation component with Link elements
- Custom CSS styling

**Technical Requirements:**
- Function-based components only (no class components)
- .jsx file extension for components
- React functionality limited to course material

**Concepts:** React framework, JSX syntax, component lifecycle, hooks (useState), client-side routing, Single Page Applications (SPAs), component composition

---

### Assignment 9: MERN Stack Exercise Tracker PORTFOLIO PROJECT
**Files:** Full-stack application (frontend-react + backend-rest)  
**Topics:** MERN stack, full-stack development, React, Node.js, Express, MongoDB  
**Description:** **Course Portfolio Assignment** - Complete full-stack MERN application for tracking exercises. Can be posted publicly on GitHub/portfolio after term ends.

**Stack:**
- **M**ongoDB - Database persistence
- **E**xpress - Backend REST API framework
- **R**eact - Frontend SPA user interface
- **N**ode.js - JavaScript runtime

**Data Model:**
- **Exercise Properties:** name (String), reps (Number), weight (Number), unit (String: "kgs"/"lbs"/"miles"), date (String, optional)

**Frontend (React):**
- Home/Retrieve Page - Display all exercises in table
- Create Page - Form to add new exercise
- Update Page - Edit existing exercise
- Navigation component
- React Router for page routing
- Fetch API for backend communication
- Custom CSS styling (reuse Assignment 2 styles)

**Backend (Node/Express/MongoDB):**
- REST API with full CRUD operations
- `POST /exercises` - Create exercise
- `GET /exercises` - Retrieve all exercises
- `PUT /exercises/:id` - Update exercise
- `DELETE /exercises/:id` - Delete exercise
- Input validation (express-validator or custom)
- MongoDB connection via Mongoose
- Environment variables (.env file)

**Features:**
- Full-stack application with separate frontend/backend
- Form validation on both client and server
- Success/failure alerts
- Automatic navigation after operations
- Date formatting (YYYY-MM-DD display)
- Professional UI/UX design

**Concepts:** MERN stack architecture, client-server communication, REST API integration, Fetch API, useEffect hook, useNavigate hook, environment configuration, full-stack deployment, cross-origin requests

---

## Technologies Used

### Front-End:
- **HTML5** - Semantic markup and structure
- **CSS3** - Styling, layout, flexbox
- **JavaScript (ES6+)** - Client-side programming, DOM manipulation
- **React** - Component-based UI framework
- **React Router** - Client-side routing

### Back-End:
- **Node.js** - JavaScript runtime environment
- **Express.js** - Web application framework
- **REST API** - Architectural style for web services
- **MongoDB** - NoSQL document database
- **Mongoose** - MongoDB object modeling (ODM)

### Tools & Libraries:
- **Jest** - JavaScript testing framework
- **VS Code** - Development environment
- **Browser DevTools** - Debugging and inspection
- **npm** - Package management
- **Vite** - Build tool and development server
- **express-validator** - Input validation

---

## How to Run

### HTML/CSS Assignments (A2):
```bash
# Open files directly in browser
open index.html
# or
open contact.html
```

### JavaScript Assignments (A3, A4):
```bash
cd assignment-folder
npm install
npm test
```

### DOM Assignment (A5):
```bash
cd assignment5
npm install
npm start
# Visit http://localhost:3000 in browser
```

### REST API Assignment (A6):
```bash
cd assignment6
npm install
npm start
# Test API using a6-test-requests.http or Postman
```

### Database API Assignment (A7):
```bash
cd assignment7
# Add MongoDB connection string to .env file
npm install
npm start
# Test API using a7-test-requests.http
```

### React SPA Assignment (A8):
```bash
cd assignment8
npm install
npm run dev
# Visit http://localhost:5173 in browser
```

### MERN App Assignment (A9):
```bash
# Backend
cd backend-rest
# Add MongoDB connection string to .env file
npm install
npm start

# Frontend (in separate terminal)
cd frontend-react
npm install
npm run dev
# Visit http://localhost:5173 in browser
```

---

## Course Information

**Course:** CS 290 - Web Development  
**Institution:** Oregon State University  
**Term:** Fall 2024  
**Technologies:** HTML, CSS, JavaScript, React, Node.js, Express, MongoDB

---

## Key Concepts Covered

### Front-End Development:
- HTML5 semantic elements and document structure
- CSS styling, box model, and responsive design
- JavaScript fundamentals (data types, functions, control flow)
- DOM manipulation and event handling
- Form validation and user interaction
- Client-side JavaScript execution
- React component architecture
- State management and hooks
- Single Page Applications (SPAs)
- Client-side routing

### Back-End Development:
- Node.js server-side JavaScript
- Express framework and routing
- REST API design and implementation
- HTTP protocol (methods, headers, status codes)
- MVC architecture pattern
- JSON data handling
- Asynchronous programming
- Database integration
- MongoDB and Mongoose ODM
- Input validation and error handling

### Full-Stack Development:
- MERN stack architecture
- Client-server communication
- REST API integration
- Environment configuration
- Cross-origin requests
- Full-stack application deployment

### Software Engineering:
- Test-driven development (TDD)
- Debugging with browser DevTools
- Version control and project organization
- Code modularity and separation of concerns
- API design best practices
- Database schema design

---

## Assignment Progression

The assignments build upon each other progressively:

1. **Assignment 1:** Understanding web fundamentals (HTTP, browsers)
2. **Assignment 2:** Creating static web pages (HTML/CSS)
3. **Assignment 3:** Adding logic with JavaScript
4. **Assignment 4:** Advanced JavaScript (functional & OOP)
5. **Assignment 5:** Making pages interactive (DOM/Events)
6. **Assignment 6:** Building back-end APIs (Node/Express)
7. **Assignment 7:** Database persistence (MongoDB/Mongoose)
8. **Assignment 8:** Building modern UIs (React/SPAs)
9. **Assignment 9:** Full-stack MERN application (complete web app)

---

*These programs demonstrate full-stack web development proficiency, from front-end design through back-end API implementation to database integration, culminating in a complete MERN stack application suitable for portfolio presentation.*
```

---
