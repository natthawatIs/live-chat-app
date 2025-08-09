# Live Chat App  

A fullstack chat application built with **React, Express, MongoDB, and Socket.io**. This project includes a **backend** (Node.js with Express) and a **frontend** (React with Vite).  

## 🚀 Live Demo  
[Click here to try the app](https://fullstack-chat-app-t3vl.onrender.com)  

## Features  

- **Authentication**: User login and registration with JWT authentication.  
- **Real-time messaging**: Powered by **Socket.io**.  
- **Media uploads**: Integrated with **Cloudinary** for image uploads.  
- **State management**: Uses **Zustand** for managing authentication and chat state.  
- **Styled with TailwindCSS**: Responsive and modern UI.  

## Project Structure  

```
fullstack-chat-app
├── backend
│   ├── src
│   │   ├── controllers        # Business logic (Auth & Message controllers)
│   │   ├── lib                # Utilities (Database, Cloudinary, Socket, Helpers)
│   │   ├── middleware         # Authentication middleware
│   │   ├── models             # Mongoose models (User & Message)
│   │   ├── routes             # API routes (Auth & Messages)
│   │   ├── seeds              # Database seeding (Sample users)
│   │   ├── index.js           # Main server file
│   ├── package.json           # Dependencies & scripts
│   ├── .env                   # Environment variables
├── frontend
│   ├── src
│   │   ├── components         # UI components (Navbar, Chat, Sidebar, etc.)
│   │   ├── pages              # Application pages (Login, Chat, Profile, etc.)
│   │   ├── store              # Zustand stores for state management
│   │   ├── lib                # Utilities (Axios, Helpers)
│   │   ├── main.jsx           # React entry point
│   ├── package.json           # Dependencies & scripts
│   ├── vite.config.js         # Vite configuration
├── package.json               # Root project configuration
├── README.md                  # Project documentation
```

## Tech Stack  

### Backend  
- **Node.js** with **Express.js**  
- **MongoDB** with **Mongoose**  
- **Socket.io** for real-time messaging  
- **JWT** for authentication  
- **Cloudinary** for media storage  

### Frontend  
- **React 19** with **Vite**  
- **React Router** for navigation  
- **Zustand** for state management  
- **TailwindCSS** for styling  
- **Socket.io Client** for real-time updates  

## Installation  

### Prerequisites  
- **Node.js** (>= 16)  
- **MongoDB** (local or cloud instance)  
- **Cloudinary** account (for image uploads)  

### Setup  

1. **Clone the repository**  
   ```sh
   git clone https://github.com/nattawatIs/fullstack-chat-app.git
   cd fullstack-chat-app
   ```

2. **Backend setup**  
   ```sh
   cd backend
   npm install
   ```

   Create a `.env` file in `backend/` and add the following:  
   ```env
   MONGO_URL=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
   CLOUDINARY_API_KEY=your_cloudinary_api_key
   CLOUDINARY_API_SECRET=your_cloudinary_api_secret
   ```

   Start the backend server:  
   ```sh
   npm run dev
   ```

3. **Frontend setup**  
   ```sh
   cd ../frontend
   npm install
   ```

   Start the frontend development server:  
   ```sh
   npm run dev
   ```

4. **Run the application**  
   - Backend: `http://localhost:5001`  
   - Frontend: `http://localhost:5173`  

## Usage  

- **Register/Login** to access the chat.  
- **Send messages** in real time.  
- **Update profile & settings**.  

## Scripts  

### Backend  
| Script       | Description                     |  
|-------------|---------------------------------|  
| `npm run dev`  | Run the backend with Nodemon  |  
| `npm start`    | Start the backend server      |  

### Frontend  
| Script         | Description                     |  
|---------------|---------------------------------|  
| `npm run dev`  | Run the frontend in dev mode   |  
| `npm run build` | Build the frontend for production |  
| `npm run preview` | Preview the built frontend  |  
