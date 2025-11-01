# 🌍TRAVEL-GO

*TRAVEL-GO* is a smart and interactive travel itinerary planner built using Node.js, Express, and MySQL. It allows users to log in, create personalized trips, manage day-wise activities, and save itineraries for future reference. The app provides destination-specific pages such as Kerala and Rajasthan, featuring beautiful images and a user-friendly drag-and-drop interface for managing trip plans.

## ✨ Features

✅ **User Authentication**  
- Secure login/signup using bcrypt  
- Session-based authentication  

✅ **Trip Management**  
- Create trips with destination and date selection  
- Store trip data in MySQL  

✅ **Dynamic Itinerary Builder**  
- Real-time drag-and-drop functionality (Rajasthan, Kerala pages)  
- Save updated order to backend via `/api/itineraries`  

✅ **Interactive UI**  
- Clean, responsive design with EJS & HTML templates  
- Image-rich pages showcasing destinations  

✅ **Data Persistence**  
- MySQL tables for users, trips, and itineraries

## 📁 Folder Structure
```
Travel-Go/
├── public/
│   ├── js/
│   │   ├── kerala.js
│   │   └── raja.js
│   ├── src/
│   │   ├── Alleppy.jpg
│   │   ├── Kochi.jpg
│   │   ├── Munnar.jpg
│   │   ├── Thrissur.jpg
│   │   ├── Wayanad.jpg
│   │   ├── goa.jpg
│   │   ├── jaipur.jpg
│   │   ├── jaisa.jpg
│   │   ├── jodh.jpg
│   │   ├── kerala.jpg
│   │   ├── kovalam.jpg
│   │   ├── maharashtra.jpg
│   │   ├── push.jpg
│   │   ├── rajasthan.jpg
│   │   ├── udaipur.jpg
│   │   └── umaid.jpg
│   ├── login.html
│   ├── signup.html
│   └── startplanning.html
├── views/
│   ├── index.ejs
│   ├── kerala.ejs
│   ├── rajasthan.ejs
│   ├── trip.ejs
│   ├── saved-itinerary.ejs
│   ├── login.ejs
│   └── signup.ejs
├── .env
├── mysql-db.txt
├── app.js
└── README.md
```
## 💻 Tech Stack

### 🎨 Frontend
- **EJS Templates** for dynamic rendering  
- **HTML5**, **CSS3**, **JavaScript**  
- **Sortable.js** for drag-and-drop itinerary management  

### ⚙️ Backend
- **Node.js** (with **Express.js** framework)  
- **MySQL2** for database connections and queries  
- **bcrypt** for password hashing and authentication  
- **express-session** for session management  
- **dotenv** for environment variable configuration  

## ⚙️ Installation and Setup

### 1️⃣ Clone the repository
`git clone https://github.com/rac521/TRAVEL-GO.git`

### 2️⃣ Navigate into the project folder
`cd TRAVEL-GO`

### 3️⃣ Install dependencies
`npm install express mysql2 ejs dotenv body-parser bcrypt express-session`
(Optional) Install nodemon for auto-reload during development
`npm install -g nodemon`

### 4️⃣ Create a .env file in the project root and add:
`DB_HOST=localhost
DB_USER=yourusername
DB_PASSWORD=yourpassword
DB_NAME=india_trip_planner
PORT=3000`

### 5️⃣ Import the MySQL database
Open MySQL and import the script from mysql-db.txt

### 6️⃣ Start the application
`node app.js`
or
`nodemon app.js`

### 7️⃣ Open the app in your browser
`http://localhost:3000`

## 🚀 Usage

Once the server is running, open your browser and log in or sign up.  
Choose your destination (Kerala or Rajasthan), view recommended activities, and customize your itinerary using drag-and-drop.  
Save your plan, and it will be securely stored in the MySQL database for future access.


## 🚧 Future Enhancements

- Integration with Google Maps API for live route visualization.  
- Add weather updates and trip cost estimations.  
- Share itineraries with friends or export as PDF.  
- Advanced search filters and user profile features.

## 👩‍💻 Author

Developed by **Rachel Reegan**(Team Lead), **Sivani J Panicker**, **Kanishka Venugopal** & **Sandra P Nellissery** as part of a Database Management System Mini Project.  
This project demonstrates full-stack integration using Node.js, Express, MySQL, and EJS to create a seamless travel planning experience.

## 📄 License

Licensed under the MIT License – you’re free to use, modify, and distribute this project.
