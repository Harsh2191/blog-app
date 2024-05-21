const fs = require('fs');

const readmeContent = `
# Blog Application

This Blog Application is a full-stack web application that allows users to create, edit, and delete blog posts. The application includes user authentication using JWT (JSON Web Token) and features a user-friendly interface built with React.js, CSS, and HTML. The backend is powered by Node.js, Express, and MongoDB.

## Features

- **User Authentication**: Secure user login and registration using JWT.
- **Create Posts**: Authenticated users can create new blog posts.
- **Edit Posts**: Users can edit their own posts.
- **Delete Posts**: Users can delete their own posts.
- **Responsive Design**: The application is designed to be responsive and mobile-friendly.

## Screenshots

### Home Page
![Home Page](path/to/homepage-screenshot.png)

### Create Post
![Create Post](path/to/create-post-screenshot.png)

### Edit Post
![Edit Post](path/to/edit-post-screenshot.png)

### User Authentication
![User Authentication](path/to/user-authentication-screenshot.png)

## Technologies Used

- **Frontend**:
  - React.js
  - CSS
  - HTML
- **Backend**:
  - Node.js
  - Express
  - MongoDB
  - JWT (JSON Web Token)

## Installation

1. Clone the repository:
   \`\`\`sh
   git clone https://github.com/yourusername/blog-application.git
   \`\`\`

2. Navigate to the project directory:
   \`\`\`sh
   cd blog-application
   \`\`\`

3. Install frontend dependencies:
   \`\`\`sh
   cd client
   npm install
   \`\`\`

4. Install backend dependencies:
   \`\`\`sh
   cd ../server
   npm install
   \`\`\`

5. Create a \`.env\` file in the \`server\` directory and add your MongoDB URI and JWT secret:
   \`\`\`env
   MONGO_URI=your_mongo_db_uri
   JWT_SECRET=your_jwt_secret
   \`\`\`

6. Start the backend server:
   \`\`\`sh
   npm start
   \`\`\`

7. Start the frontend development server:
   \`\`\`sh
   cd ../client
   npm start
   \`\`\`

## Usage

1. Open the browser and navigate to \`http://localhost:3000\`.
2. Register a new account or log in with existing credentials.
3. Create, edit, and delete your blog posts.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes. For major changes, please open an issue to discuss what you would like to change.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
`;

fs.writeFile('README.md', readmeContent, (err) => {
  if (err) throw err;
  console.log('README.md has been created!');
});

 
 
