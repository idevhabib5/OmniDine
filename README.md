# OmniDine
Full-Stack Restaurant Management System (MERN)
A robust, end-to-end solution for modern restaurant operations. This platform bridges the gap between front-of-house service, kitchen coordination, and back-office administration using real-time data synchronization.

🚀 Core Modules
📱 Staff & Operations (Frontend)
Live Table Management: Interactive floor plan using CSS Grid/Canvas to track real-time table statuses (Available, Occupied, Dirty).

Digital Waiter Pad: Optimized mobile-first interface for rapid order entry with customizable modifiers.

Kitchen Display System (KDS): Real-time order queue with status toggles (Pending → Preparing → Ready) powered by Socket.io.

💼 Administrative Suite (Frontend)
Dynamic Menu Builder: Full CRUD functionality for menu items, including category management and image uploads.

Business Intelligence: Visualized sales analytics and inventory movement using Recharts.

RBAC (Role-Based Access Control): Secure dashboard access restricted to Admin and Manager roles.

⚙️ The Engine (Backend)
RESTful API: Scalable Node/Express architecture with structured routing.

State Persistence: MongoDB (Mongoose) for flexible document storage of complex orders and menu schemas.

Security: JWT-based authentication and Bcrypt password hashing.

🛠️ Tech Stack
Frontend: React.js, Redux Toolkit (State Management), Tailwind CSS (UI), Framer Motion (Animations). Backend: Node.js, Express.js. Database: MongoDB. Real-time: Socket.io. Tools: Postman (API Testing), Docker (Containerization).

🏗️ Database Schema Overview
The system relies on a relational-style document design to ensure data integrity:

Users: Roles, credentials, and activity logs.

Menu: Item details, pricing, categories, and availability.

Tables: Seat capacity, location, and current session ID.

Orders: Linked to Tables and Users, containing item arrays, timestamps, and payment status.

🚦 Getting Started
1. Prerequisites
Node.js (v16+)

MongoDB Atlas account or local Compass instance.

2. Installation
Bash
# Clone the repository
git clone https://github.com/your-username/restaurant-management-mern.git

# Install dependencies for Backend
cd backend
npm install

# Install dependencies for Frontend
cd ../frontend
npm install
3. Environment Setup
Create a .env file in the backend directory:

Code snippet
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
4. Run the Application
Bash
# Run backend (from /backend)
npm run dev

# Run frontend (from /frontend)
npm start
