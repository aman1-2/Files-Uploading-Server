# Project Description: File Upload Management System

## Overview
This project aims to create a robust file upload management system utilizing Node.js, Express.js, MongoDB, and Cloudinary. It facilitates the seamless upload of various file types, such as images and videos, to either local or cloud servers while ensuring data validation and integrity.

## Project Structure

### Config Folder
- **cloudinary.js**: Configures Cloudinary settings for file storage and retrieval.
- **database.js**: Establishes a connection to the MongoDB database.

### Controllers Folder
- **uploadController.js**: Handles file upload operations, including local file upload, image upload to Cloudinary, video upload to Cloudinary, and image size reduction for Cloudinary.

### Models Folder
- **file.js**: Defines the Mongoose schema for storing file details in the MongoDB database. Implements middleware for sending email notifications upon successful file uploads.

### Routes Folder
- **fileUpload.js**: Defines API routes for file upload operations.

### Other Files
- **.env**: Stores environment variables such as database URL, Cloudinary credentials, and mail server configuration.
- **index.js**: Main entry point of the application. Configures Express server, establishes database and Cloudinary connections, defines routes, and launches the server.

## Features
- **Local File Upload**: Supports uploading files to the local server with validation and storage in a designated folder.
- **Image and Video Upload to Cloudinary**: Enables uploading images and videos to Cloudinary cloud storage with validation and automatic resizing.
- **Email Notification**: Sends email notifications to users upon successful file uploads.
- **Data Validation**: Ensures that only supported file types are uploaded and processed.
- **Middleware**: Utilizes pre and post middleware for executing actions before and after database operations, enhancing functionality and scalability.

## Getting Started
1. Clone the repository to your local machine.
2. Install dependencies using `npm install`.
3. Set up environment variables in the `.env` file.
4. Run the application using `npm start`.
5. Access the API endpoints to perform file upload operations.

## Dependencies
- **Express.js**: Web framework for Node.js.
- **Mongoose**: MongoDB object modeling for Node.js.
- **Cloudinary**: Cloud-based image and video management platform.
- **Nodemailer**: Module for sending emails from Node.js applications.
- **dotenv**: Loads environment variables from a `.env` file into `process.env`.

## Contributors
- Aman Pratap Singh

## License
This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).