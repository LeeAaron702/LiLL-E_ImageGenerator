# LiLL-E Image Generator 

## Introduction 

LiLL-E Image Generator is a full-stack web application that leverages the power of OpenAi DALL-E to generate images based on provided prompts.  The application is divided into a client side and a server side.

## Features
The main features of this application include:

- User can input a prompt and the application will generate an image based on that prompt.
- The generated images are stored and can be retrieved for later use.
- Generated images can be downloaded and saved 

## Technologies 

### Client Side 
- React.js: A JavaScript library for building user interfaces, especially single-page applications. React is the main technology used for building the front-end of this application.
- File-saver: A solution for client-side file saving that is not dependent on any server-side solutions. It's used to enable users to save files on the client side.
- React Router DOM: A package that provides DOM bindings for React Router, which is used for routing in React applications. It's used for managing and implementing routing on the client side.
- Vite: A modern web dev build tool that allows for faster and leaner development. It's used for building and serving the client side application.
- ESLint: A pluggable and configurable linter tool for identifying and reporting on patterns in JavaScript. It's used for enforcing code style and catching potential bugs before runtime.
- Tailwind CSS: A utility-first CSS framework for rapidly building custom designs. It's used for styling the client side application.
- PostCSS: A tool for transforming CSS with JavaScript. It's used for processing CSS.
- Autoprefixer: A PostCSS plugin to parse CSS and add vendor prefixes to CSS rules using values from the Can I Use website. It's used to ensure compatibility across different browsers.
- Hostinger: Frontend Deployment 


### Server Side 
- Node.js: A JavaScript runtime built on Chrome's V8 JavaScript engine, used for building scalable network applications.
- Express.js: A fast, unopinionated, and minimalist web framework for Node.js. Express is used to build the web server for the application.
- Mongoose: An Object Data Modeling (ODM) library for MongoDB and Node.js. It manages relationships between data, provides schema validation, and is used to translate between objects in code and the representation of those objects in MongoDB.
- Cloudinary: A cloud-based service that provides an end-to-end image and video management solution including uploads, storage, manipulations, optimizations and delivery. It's used for managing images in the application.
- OpenAI: An artificial intelligence research lab consisting of both for-profit and non-profit arms. The OpenAI API provides a way to generate human-like text, and in this application, it is likely used as part of the image generation process.
- dotenv: A module that loads environment variables from a .env file into process.env. It's used for managing environment variables in the application.
- cors: A Node.js package for providing a Connect/Express middleware that can be used to enable CORS with various options.
- nodemon: A utility that will monitor for any changes in the server source and automatically restart the server. This is used in a development environment​1​​2​.
- Render.com: Backend hosting

### Database 
- Atlas MongoDB

## Structure
The application is divided into two main parts: the client side and the server side.

### Client Side
The client side of the application is built using React.js. The code for the client side is located in the client directory.

### Server Side
The server side of the application is built using Node.js and Express.js. It also utilizes Mongoose for database operations and Cloudinary for image management. The code for the server side is located in the server directory.

### Setup
To set up the application, follow the steps below:

### Clone the repository.
```
Navigate to the client directory and run npm install to install all client side dependencies.
Navigate to the server directory and run npm install to install all server side dependencies.
```
### Usage
To use the application, follow the steps below:
```
In the client directory, run npm run dev to start the development server.
In the server directory, run npm run start to start the server.
```

## Database Schema
The application uses a MongoDB database. The schema for the database is as follows:

### Post Schema:
```
{
  name: { type: String, required: true},  
  prompt: { type: String, required: true},  
  photo: { type: String, required: true},  
}
```



