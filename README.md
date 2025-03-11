# SIT737-2025-Prac2p: Simple Web Server with Node.js and Express

This repository contains a simple web server built using Node.js and the Express framework. It serves a basic HTML page when accessed at the root URL (`/`).

## Prerequisites
- Node.js installed (verify with `node -v`)
- Git installed for version control

## Setup Instructions
1. **Initialize the Project**:
   - Create a directory: `mkdir sit737-2025-prac2p`
   - Navigate into it: `cd sit737-2025-prac2p`
   - Initialize a Node.js project: `npm init -y`

2. **Install Express**:
   - Run: `npm install express`

3. **Create the Server**:
   - Create a file named `server.js` and add the code provided below.
   - The server listens on port 3000 and serves a simple HTML page.

4. **Run the Server**:
   - Execute: `node server.js`
   - Open a browser and visit: `http://localhost:3000`

## Code Explanation
- **server.js**:
  ```javascript
  const express = require('express');
  const app = express();
  const port = 3000;

  app.get('/', (req, res) => {
    res.send(`<html>...</html>`); // Simplified HTML content
  });

  app.listen(port, () => {
    console.log(`Server is running at http://localhost:${port}`);
  });

  
#### Step 5: Push to GitHub
1. **Initialize a Git Repository**:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Simple web server with Express"
