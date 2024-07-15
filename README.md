# CONNECTVERSE
```markdown
# Connectverse

Connectverse is a web application with secure user authentication built using React.js, Node.js, Express.js, MongoDB, and JWT.

## Features

- User Registration and Authentication
- JWT-based Authentication
- Secure Password Storage
- Responsive Design with Tailwind CSS
- Password Reset Functionality
- Email Verification
- Accessibility Enhancements

## Technology Stack

- React.js
- Node.js
- Express.js
- MongoDB
- JWT (jsonwebtoken)
- Tailwind CSS

## Prerequisites

- Node.js (v14.x or higher)
- npm (v6.x or higher)
- MongoDB

## Project Setup

### Backend Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/connectverse.git](https://github.com/suryasivakumar22/CONNECTVERSE-USING-EXPRESS-NODE-BACKEND-API.git
   cd connectverse
   ```

2. Install backend dependencies:
   ```bash
   cd server
   npm install
   ```

3. Create a `.env` file in the `server` directory and add your environment variables:
   ```env
   PORT=5000
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   ```

4. Run the backend server:
   ```bash
   npm start
   ```

### Frontend Setup

1. Navigate to the frontend directory and install dependencies:
   ```bash
   cd ../client
   npm install
   ```

2. Create a `tailwind.config.js` file in the `client` directory:
   ```js
   module.exports = {
     purge: ['./src/**/*.{js,jsx,ts,tsx}', './public/index.html'],
     darkMode: false, // or 'media' or 'class'
     theme: {
       extend: {},
     },
     variants: {
       extend: {},
     },
     plugins: [],
   };
   ```

3. Create a `postcss.config.js` file in the `client` directory:
   ```js
   module.exports = {
     plugins: {
       tailwindcss: {},
       autoprefixer: {},
     },
   };
   ```

4. Create a `src/globals.css` file and add Tailwind imports:
   ```css
   @import 'tailwindcss/base';
   @import 'tailwindcss/components';
   @import 'tailwindcss/utilities';

   :root {
     --font-heading: 'Manrope', sans-serif;
     --font-body: 'Manrope', sans-serif;
   }

   body {
     font-family: var(--font-body);
   }

   .antialiased {
     -webkit-font-smoothing: antialiased;
     -moz-osx-font-smoothing: grayscale;
   }

   .font-heading {
     font-family: var(--font-heading);
   }

   .font-body {
     font-family: var(--font-body);
   }
   ```

5. Start the frontend development server:
   ```bash
   npm start
   ```

### Running the Application

1. Ensure the backend server is running.

2. Run the frontend development server:
   ```bash
   npm start
   ```

3. Open your browser and navigate to `http://localhost:3000` to view the application.

