# QuickShow - FullStack Movie Booking Application

QuickShow is a modern, full-stack web application for booking movie or show tickets. Built with a robust MERN-like stack featuring modern tooling, authentication, and payment integrations.

## 🚀 Tech Stack

### Frontend (Client)
- **Framework:** React 19 (via Vite)
- **Routing:** React Router DOM
- **Styling:** Tailwind CSS
- **Authentication:** Clerk React
- **HTTP Client:** Axios
- **Media:** React Player

### Backend (Server)
- **Framework:** Express.js (Node.js)
- **Database:** MongoDB (Mongoose)
- **Authentication:** Clerk Express
- **Payments:** Stripe
- **Background Jobs:** Inngest
- **Image Storage:** Cloudinary
- **Emails:** Nodemailer
- **Webhooks:** Svix

## 📁 Project Structure

The project is structured as a monorepo containing both the frontend client and the backend server.

- `/client` - The Vite + React frontend application.
- `/server` - The Express.js backend API.

## ⚙️ Prerequisites

Make sure you have the following installed:
- Node.js (v18 or higher recommended)
- MongoDB instance (Local or Atlas)
- Accounts for Clerk, Stripe, Cloudinary, and Inngest.

## 🛠️ Getting Started

### 1. Clone the repository
\`\`\`bash
git clone https://github.com/nikhilgetitdone2027/QuickShow-FullStack.git
cd QuickShow-FullStack
\`\`\`

### 2. Setup the Server
Navigate to the server directory and install dependencies:
\`\`\`bash
cd server
npm install
\`\`\`

Create a `.env` file in the `server` directory and configure the necessary environment variables:
\`\`\`env
# Database
MONGODB_URI=your_mongodb_connection_string

# Authentication (Clerk)
CLERK_SECRET_KEY=your_clerk_secret_key
CLERK_WEBHOOK_SECRET=your_clerk_webhook_secret

# Payments (Stripe)
STRIPE_SECRET_KEY=your_stripe_secret_key
STRIPE_WEBHOOK_SECRET=your_stripe_webhook_secret

# Cloudinary
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret

# Emails (Nodemailer)
EMAIL_USER=your_email_address
EMAIL_PASS=your_email_app_password
\`\`\`

Start the server:
\`\`\`bash
npm run server
\`\`\`
The server will run on `http://localhost:3000`.

### 3. Setup the Client
Open a new terminal, navigate to the client directory, and install dependencies:
\`\`\`bash
cd client
npm install
\`\`\`

Create a `.env` file in the `client` directory:
\`\`\`env
VITE_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
VITE_API_URL=http://localhost:3000
\`\`\`

Start the development server:
\`\`\`bash
npm run dev
\`\`\`
The client will usually run on `http://localhost:5173`.

## 📜 Available Scripts

### Client
- `npm run dev`: Starts the Vite development server.
- `npm run build`: Builds the application for production.
- `npm run preview`: Previews the production build locally.
- `npm run lint`: Runs ESLint to check for code issues.

### Server
- `npm start`: Starts the server using Node.
- `npm run server`: Starts the server in development mode using Nodemon.

## 🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License
This project is licensed under the ISC License.
