# TrelloLite - Modern Task Manager

A full-stack, premium Kanban-style task manager built with Next.js and MongoDB.

## Features

- **User Authentication**: Secure JWT-based login/signup with cookie storage.
- **Drag & Drop**: Intuitive task management using `@hello-pangea/dnd`.
- **Priority System**: Mark tasks as "High Priority" for special highlighting and automatic top-of-list placement. ⭐
- **Due Date Reminders**: Visual indicators for upcoming and overdue tasks. ⏰
- **Premium UI**: Glassmorphism aesthetic, responsive design, and smooth animations using Framer Motion.
- **Dark Mode**: Fully supported dark/light theme toggle.
- **Persistence**: All tasks and user data stored in MongoDB using Mongoose.

## Tech Stack

- **Frontend**: Next.js (Pages Router), Tailwind CSS, Lucide Icons, Framer Motion.
- **Backend**: Next.js API Routes, JWT, Bcrypt.js.
- **Database**: MongoDB with Mongoose ODM.

## Prerequisites

- Node.js 18+ 
- MongoDB URI (local or MongoDB Atlas)

## Setup Instructions

1. **Clone the project**
   ```bash
   git clone <repository-url>
   cd trello-lite
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Environment Variables**
   Create a `.env.local` file in the root directory and add the following:
   ```env
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET=your_random_secret_string
   ```

4. **Run Development Server**
   ```bash
   npm run dev
   ```

5. **Access the application**
   Open [http://localhost:3000](http://localhost:3000) in your browser.

## Deployment

This app is ready to be deployed on **Vercel**. 
- Connect your GitHub repo to Vercel.
- Add the `MONGODB_URI` and `JWT_SECRET` environment variables in the Vercel project settings.
- Deploy!

## Folder Structure

- `/components`: Reusable UI components (TaskCard, Navbar, etc.)
- `/pages`: Next.js pages and API routes
- `/lib`: Helper functions, utilities, and context providers
- `/models`: Mongoose schemas for data modeling
- `/styles`: Global CSS and theme configurations
