# 🎄 **Carolling Tracker** - A Christmas Fund Tracker with Spring Boot & Vue.js 🎶

**Carolling Tracker** is a web-based application to help carolling groups track the money received during their holiday activities. The application allows users to upload donation data in CSV format, display the information in a user-friendly table, and download the updated data. The backend is powered by **Spring Boot**, and the frontend is built using **Vue.js**, making the app both dynamic and easy to use.

## Features

- **Upload CSV**: Easily upload CSV files containing donation records (date, caroller, amount).
- **View Donations**: Display a table of donations and carollers, with the ability to edit data.
- **Export Data**: Download the updated donation data as a CSV file after processing.
- **Responsive Design**: Works seamlessly across desktop and mobile devices.
- **Interactive Frontend**: Built with Vue.js to provide a dynamic user interface.

## Tech Stack

- **Frontend**: Vue.js (for building a reactive and modern user interface)
- **Backend**: Spring Boot (Java-based backend for handling API requests)
- **Database**: CSV-based storage for simplicity (can be replaced with a database like MySQL or MongoDB)
- **API**: RESTful API (Spring Boot) for communication between backend and frontend
- **Deployment**: Can be deployed on platforms like **Heroku**, **AWS**, or **Vercel**

## File Structure
```md
carolling-tracker/
├── backend/                      # Spring Boot Backend
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── com/
│   │   │   │       └── carollingtracker/
│   │   │   │           ├── CarollingTrackerApplication.java  # Main Spring Boot Application
│   │   │   │           ├── controller/                      # Controller to handle file upload & data retrieval
│   │   │   │           ├── model/                           # Model for donation records
│   │   │   │           └── service/                         # Service to process CSV data
│   │   │   └── resources/
│   │   │       ├── application.properties                    # Spring Boot configuration
│   │   │       └── static/                                    # Static assets (Vue.js build output)
│   ├── pom.xml                                                   # Maven dependencies for backend
│
├── frontend/                    # Vue.js Frontend
│   ├── src/
│   │   ├── assets/                                            # Static assets (images, etc.)
│   │   ├── components/                                        # Vue.js components
│   │   │   └── DonationTable.vue                               # Table component to show donation data
│   │   ├── views/
│   │   │   └── Home.vue                                         # Main view for displaying and uploading CSVs
│   │   ├── App.vue                                              # Main Vue component
│   │   ├── main.js                                              # Vue.js entry point for app
│   ├── public/                                                  # Public assets (e.g., index.html)
│   ├── package.json                                             # NPM dependencies for frontend
│   └── vue.config.js                                            # Configuration for Vue.js, e.g., proxy setup for API requests
│
└── README.md                                                     # Project documentation (this file)
```

---

## Project Structure

The project consists of two main parts: the **backend** (Spring Boot) and the **frontend** (Vue.js).
