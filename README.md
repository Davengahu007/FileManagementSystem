# File Management System

## Introduction
This project is a File Management System designed to organize and manage digital files within a structured directory. It allows users to create, delete, and navigate through directories and manage files, including uploading, downloading, renaming, and deleting files.

## Features
- **Directory Management**: Create, delete, and browse directories.
- **File Operations**: Upload, download, rename, and delete files.
- **Dynamic Navigation**: Navigate through directories and view their contents.
- **File Previews**: Preview file details before downloading.

## Technologies Used
- **Backend**: Node.js, Express.js
- **Frontend**: React.js with Tailwind CSS for styling
- **Database**: MongoDB/PostgreSQL (choose based on your setup)
- **API Testing**: Postman for API route testing

## Setup Instructions

### Prerequisites
- Node.js
- npm or yarn
- MongoDB or PostgreSQL
- Git (optional)

### Backend Setup
1. Clone the repository (if using Git):
   ```git clone https://your-repository-url.com cd FileManagementSystem```

2. Install Dependendcies
   ```cd backend npm install```

3. Configure your database:
- Ensure that your database service is running.
- Configure the database connection settings in `config.js` or through environment variables.

4. Start the server:
   ```npm start```


### Frontend Setup
1. Navigate to the frontend directory:
   ```cd frontend```

2. Install dependencies:
   ```npm install```

3. Start the React application:
   ```npm start```

- The application will run on `http://localhost:3000`.

## API Endpoints

### Directories
- **GET /api/directories/all** - Retrieve all directories.
- **GET /api/directories/** - Retrieve all top-level directories.
- **GET /api/directories/{id}** - Retrieve a specific directory by ID.
- **GET /api/directories/{id}/children** - Retrieve all child directories of a specific directory.
- **GET /api/directories/{id}/files** - Retrieve all files within a specific directory.
- **POST /api/directories/** - Create a new directory.
- **PUT /api/directories/{id}** - Update a specific directory.
- **DELETE /api/directories/{id}** - Delete a specific directory.

### Files
- **GET /api/files/** - Retrieve all files.
- **GET /api/files/{id}** - Retrieve a specific file by ID.
- **POST /api/files/** - Create a new file record.
- **POST /api/files/upload** - Upload a file to a specified directory.
- **GET /api/files/files/download/{id}** - Download a specific file.
- **PUT /api/files/{id}** - Update a specific file.
- **DELETE /api/files/{id}** - Delete a specific file.

## Using the Application
- Navigate to the root URL (e.g., `http://localhost:3000`).
- Use the interface to create, delete, and navigate directories.
- Upload or download files by following the prompts on the interface.

## Future Enhancements
- Implement user authentication.
- Add file search functionality.
- Support file versioning.


