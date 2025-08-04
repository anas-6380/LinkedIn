🧑‍💼**LinkedIn Clone (MERN Stack)**
A professional networking web application built with MongoDB, Express.js, React.js, and Node.js, replicating core functionality of LinkedIn including authentication, posts, profiles, and connections.



**🚀 Features**
🔸User Authentication with email, username, JWT-based sign-up/login

🔸Create, view, and delete posts (text content + images via Cloudinary)

🔸User Profiles: first & last name, headline, skills, education, experience, profile & cover images

🔸Connections: send/accept connection requests, view mutual connections

🔸Secure Backend with protected routes, input validation, and hashed passwords (bcrypt)

🔸Cookies & Token handling for secure sessions

🔸Frontend built with React and Vite for fast hot-reloads and optimized production build

**📂 Project Structure**

LinkedIn/

├── backend/

│   ├── controllers/        // auth & post logic

│   ├── models/             // User.js, Post.js

│   ├── routes/             // auth.routes.js & post.routes.js

│   ├── config/             // token.js (JWT config)

│   ├── index.js            // server entry point

│   └── .env                // config variables (MONGODB_URL, JWT_SECRET)

└── frontend/

    ├── src/
    │   ├── pages/          // Login, Register, Home, Profile
    
    │   ├── components/     // Navbar, Feed, PostCard, etc.
    
    │   ├── context/        // UserContext.jsx (global auth state)
    
    │   ├── assets/         // Logo, icons, images
    
    │   ├── App.jsx

    
    │   └── main.jsx
    
    
    ├── public/
    

    
    ├── vite.config.js
    
    
    └── package.json
    
    
    





    
**🛠️ Setup Instructions**
🔸 _Backend (Express + MongoDB)_

🔸 _Navigate to backend:_
cd backend


🔸 _Install dependencies:_
npm install


🔸 _Create a .env file using .env.example:
PORT=8000
MONGODB_URL=<your Atlas connection string>
JWT_SECRET=<your secret>
CLOUDINARY_API_KEY=…
CLOUDINARY_API_SECRET=…
CLOUDINARY_CLOUD_NAME=…


🔸 _Start the server (with hot reload):_
npm run dev


_✅ You should see:_
server started
MongoDB connected
Frontend (React + Vite)



🔸 _Open a new terminal:_
cd frontend


🔸 _Install dependencies:_
npm install


**Configure API base URL in .env or your context (if needed).**
_Start local development:_
🔸npm run dev
Navigate to http://localhost:3000 and you’ll see the logged-in state managed via UserContext.

**☁️ Deployment**
Backend Deployment (e.g. on Render / Heroku)
🔸Set environment variables (MONGODB_URL, JWT_SECRET, PORT, CLOUDINARY_*) in service dashboard.

🔸Ensure file imports are case-sensitive (Linux environment).

🔸Start command: npm run dev or node index.js

🔸Frontend Deployment (Static Site on Render)
In Render’s static site settings:

🔸Build Command:
🔸npm install && npm run build


🔸Root Directory: frontend (if your frontend isn't at repo root)
Publish Directory: dist

🔸_Ensure imports like:_
import { UserProvider } from "./context/UserContext"
match filename casing exactly.

🧪 Troubleshooting Tips
🔹Case-sensitivity errors: rename filenames using git mv to ensure Git tracks the change (especially for UserContext.jsx).

🔹Sign-up issues: check backend logs for errors (e.g. duplicate email, validation failure) and display real error messages in frontend using console.log(err.response.data).

🔹Token failures: confirm JWT secret matches between backend and token config.

🔹Port in use: if EADDRINUSE occurs locally, either kill the process or change the port.

🧩 Additional Enhancements
🔹Add likes, comments, or real-time updates using Socket.io

🔹Integrate search, filters, or recommendation systems

🔹Improve UI design with frameworks like Tailwind CSS or Material‑UI

🔹Deploy with domain names and HTTPS support

📬 Feedback & Contribution
Contributions, bug reports, and feature suggestions are welcome!
Feel free to create issues or submit pull requests.

