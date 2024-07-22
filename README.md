

# Taskflow (Fullstack MERN Task Manager)

## Overview

Taskflow is a cloud-based task management web application designed to enhance team productivity and collaboration. Built with the MERN stack (MongoDB, Express.js, React, and Node.js), Taskflow offers a seamless and intuitive interface for efficient task assignment, tracking, and management. The platform supports both administrators and regular users, providing robust features to streamline workflow and improve organizational efficiency.

## Problem Statement

In today’s fast-paced work environments, traditional task management methods such as spreadsheets or manual tracking systems are often inefficient and error-prone. Taskflow addresses these issues by providing a centralized platform that fosters seamless collaboration and enhanced workflow efficiency.

## Background

The rise of remote work and distributed teams has highlighted the need for effective communication and task coordination tools. Taskflow meets this need by leveraging modern web technologies to deliver a responsive and scalable task management solution. The integration of Redux Toolkit, Headless UI, and Tailwind CSS ensures a superior user experience and performance.

## Features

### Admin Features

1. **User Management**
   - Create admin accounts
   - Add and manage team members

2. **Task Assignment**
   - Assign tasks to individuals or multiple users
   - Update task details and status

3. **Task Properties**
   - Label tasks as todo, in progress, or completed
   - Assign priority levels (high, medium, normal, low)
   - Add and manage sub-tasks

4. **Asset Management**
   - Upload task assets, such as images

5. **User Account Control**
   - Disable or activate user accounts
   - Permanently delete or trash tasks

### User Features

1. **Task Interaction**
   - Change task status (in progress or completed)
   - View detailed task information

2. **Communication**
   - Add comments or chat to task activities

### General Features

1. **Authentication and Authorization**
   - Secure user login
   - Role-based access control

2. **Profile Management**
   - Update user profiles

3. **Password Management**
   - Securely change passwords

4. **Dashboard**
   - Summary of user activities
   - Filter tasks into todo, in progress, or completed

## Technologies Used

### Frontend

- React (Vite)
- Redux Toolkit for State Management
- Headless UI
- Tailwind CSS

### Backend

- Node.js with Express.js

### Database

- MongoDB for efficient and scalable data storage

Taskflow is an innovative solution that brings efficiency and organization to team task management. Utilizing the MERN stack and modern frontend technologies, it provides a seamless experience for both administrators and users, promoting collaboration and productivity.

## Setup Instructions

### Server Setup

#### Environment Variables

First, create a `.env` file in the server folder containing the following environment variables:

- `MONGODB_URI`: Your MongoDB URL
- `JWT_SECRET`: Any secure secret key
- `PORT`: 8800 or any preferred port number
- `NODE_ENV`: development

#### Set Up MongoDB

1. **Visit MongoDB Atlas Website**: [https://www.mongodb.com/cloud/atlas](https://www.mongodb.com/cloud/atlas)
2. **Create an Account**: Sign up and log in to MongoDB Atlas.
3. **Create a New Cluster**: Follow the instructions to create a cluster.
4. **Configure Cluster Settings**: Choose your cloud provider and region, then create the cluster.
5. **Create Database User**: Set up your database user and configure IP whitelist.
6. **Connect to Cluster**: Obtain your MongoDB connection URL and configure it in your `.env` file.

#### Run Server

1. Open the project in your preferred editor.
2. Navigate to the server directory: `cd server`.
3. Install dependencies: `npm install`.
4. Start the server: `npm start`.

If configured correctly, the server should start successfully, and you should see a message indicating that the database is connected.

### Client Side Setup

#### Environment Variables

Create a `.env` file in the client folder containing the following environment variables:

- `VITE_APP_BASE_URL`: `http://localhost:8800` (or your server port)
- `VITE_APP_FIREBASE_API_KEY`: Your Firebase API key

#### Run Client

1. Navigate to the client directory: `cd client`.
2. Install dependencies: `npm install`.
3. Start the client: `npm start`.
4. Open [http://localhost:3000](http://localhost:3000) in your browser to view the application.
