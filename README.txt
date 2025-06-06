🩺 HEALTHCARE PATIENT MANAGEMENT SYSTEM
--------------------------------------

A full-stack web application to manage patients' medical records using React, Node.js, and MongoDB Atlas.
The system allows adding, viewing, searching, and deleting patient records with seamless database integration using MongoDB Compass.

=======================
PROJECT STRUCTURE
=======================
healthcare-patient-system/
├── backend/          -> Node.js + Express API
│   ├── app.js
│   ├── .env          -> MongoDB connection URI
│   ├── models/
│   │   └── Patient.js
│   ├── routes/
│   │   └── patients.js
│   └── package.json
├── frontend/         -> React application
│   ├── src/
│   │   └── App.js
│   └── package.json
└── README.txt

=======================
HOW TO RUN THE PROJECT
=======================

1. EXTRACT ZIP
--------------
- Extract the ZIP file.
- Open the folder in Visual Studio Code.

2. BACKEND SETUP
----------------
cd backend
npm install

Create a file `.env` in backend/ and paste your MongoDB URI:

MONGO_URI=mongodb+srv://<username>:<password>@cluster0.mongodb.net/healthcare_db?retryWrites=true&w=majority

Run the server:
node app.js

Expected output:
MongoDB Connected
Server running on port 5000

3. FRONTEND SETUP
-----------------
cd ../frontend
npx create-react-app .
npm install axios

(If src/App.js exists, overwrite with the provided one)

Run React app:
npm start

Browser opens: http://localhost:3000

4. VIEW DATA IN MONGODB COMPASS (OPTIONAL)
------------------------------------------
- Open MongoDB Compass
- Use same URI as in `.env`
- Explore `healthcare_db > patients` collection

=======================
TECHNOLOGIES USED
=======================
Frontend: React, Axios
Backend: Node.js, Express
Database: MongoDB Atlas
Tools: MongoDB Compass, VS Code

=======================
CONTACT
=======================
Developed by:Sai krishna Murali Mudunuru

You may extend this project with:
- Admin/Staff login (JWT)
- Chart-based analytics
- Export to Excel/PDF