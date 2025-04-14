# Rhythmix Music Application

A modern, responsive music streaming application built with React and Express.

## Features

- 🎵 Music player with playback controls
- 🔍 Search functionality for tracks, artists, and albums
- 📚 Library management for saved music
- 👤 User authentication system
- 📱 Responsive design for all devices
- 🌙 Dark-themed interface

## Tech Stack

- **Frontend**: React, Bootstrap, TanStack Query
- **Backend**: Express.js, Passport.js
- **Database**: Prepared for PostgreSQL with Drizzle ORM
- **Authentication**: Session-based with Passport.js

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn

### Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd rhythmix
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file in the root directory with the following variables:
   ```
   NODE_ENV=development
   PORT=5000
   SESSION_SECRET=your-secret-key
   ```

4. Start the development server:
   ```bash
   npm run dev
   ```

5. Open your browser and navigate to [http://localhost:5000](http://localhost:5000)

## Folder Structure

- `/client` - Frontend React code
  - `/src/components` - React components
  - `/src/pages` - Page components
  - `/src/hooks` - Custom React hooks
  - `/src/lib` - Utility functions and types
- `/server` - Backend Express code
- `/shared` - Shared types and schemas

## VS Code Integration

This project includes VS Code configuration files for an enhanced development experience:

- Press F5 to start the application with debugging
- Editor settings are configured for TypeScript and React development
- Proper launch configuration for debugging the server

## Authentication

The application includes a complete authentication system:

- User registration and login
- Protected routes that require authentication
- Secure password hashing
- Session management

## License

[MIT License](LICENSE)