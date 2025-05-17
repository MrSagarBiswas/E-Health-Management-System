# E-Health Management System

A full-stack web application that provides a user-friendly platform for managing medical records, scheduling appointments, real-time communication, and secure payments.

---

## Table of Contents

1. [Features](#features)  
2. [Tech Stack](#tech-stack)  
3. [Prerequisites](#prerequisites)  
4. [Getting Started](#getting-started)  
   - [Clone the Repository](#clone-the-repository)  
   - [Backend Setup](#backend-setup)  
   - [Frontend Setup](#frontend-setup)  
5. [Environment Variables](#environment-variables)  
6. [Usage](#usage)  
7. [Screenshots](#screenshots)  
8. [License](#license)  

---

## Features

- **User-Friendly Platform**  
  Browse medical records, schedule appointments, and communicate with healthcare providers via an intuitive React.js interface.  

- **Razorpay API Integration**  
  Secure direct payments of hospital bills by insurance companies using Razorpay.  

- **Real-Time Chat Engine**  
  Instant, private messaging between patients and healthcare professionals.  

- **MongoDB + Mongoose**  
  Efficient storage and retrieval of patient data, medical histories, and treatment details.  

- **Online Appointment & Payment**  
  Book appointments and pay online in a few clicks—no manual processes required.  

---

## Tech Stack

- **Frontend**: React.js, Axios  
- **Backend**: Node.js, Express  
- **Database**: MongoDB (Mongoose ODM)  
- **Payments**: Razorpay API  
- **Real-Time Chat**: Chat Engine  

---

## Prerequisites

- [Node.js (v14+)](https://nodejs.org/)  
- [npm (v6+)](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)  
- A [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) cluster URI  
- Razorpay account for API keys  

---

## Getting Started

### Clone the Repository

```bash
git clone https://github.com/MrSagarBiswas/E-Health-Management-System.git
cd E-Health-Management-System
````

### Backend Setup

1. **Navigate to the backend folder**

   ```bash
   cd backend
   ```
2. **Create a `.env` file**
   Inside `backend/`, create a file named `.env` and add your keys:

   ```env
   MONGODB_URI=your_mongodb_atlas_connection_string
   KEY_ID=your_razorpay_key_id
   KEY_SECRET=your_razorpay_key_secret
   ```
3. **Install dependencies**

   ```bash
   npm install
   ```
4. **Start the server**

   ```bash
   npm start
   ```

Your backend will run on `http://localhost:5000` (by default).

### Frontend Setup

1. **Open a new terminal and navigate to the frontend folder**

   ```bash
   cd ../frontend
   ```
2. **Create a `.env` file**
   Inside `frontend/`, create a file named `.env` and add:

   ```env
   REACT_APP_API=https://e-health-management-system.onrender.com
   REACT_APP_KEY_ID=your_razorpay_key_id
   ```
3. **Install dependencies**

   ```bash
   npm install
   ```
4. **Start the React app**

   ```bash
   npm start
   ```

Your frontend will run on `http://localhost:3000`.

---

## Environment Variables

| File            | Variable           | Description                                     |
| --------------- | ------------------ | ----------------------------------------------- |
| `backend/.env`  | `MONGODB_URI`      | MongoDB Atlas connection string                 |
|                 | `KEY_ID`           | Razorpay API key ID                             |
|                 | `KEY_SECRET`       | Razorpay API key secret                         |
| `frontend/.env` | `REACT_APP_API`    | Backend API base URL                            |
|                 | `REACT_APP_KEY_ID` | Razorpay API key ID (for payment button config) |

---

## Usage

1. Register as a **Patient** or **Insurance Company**.
2. As a patient, view/edit your medical records and book appointments.
3. Insurance companies can pay hospital bills directly through Razorpay integration.
4. Use the in-app chat to communicate with healthcare providers in real time.

---

## Screenshots

![Dashboard](https://github.com/MrSagarBiswas/E-Health-Management-System/assets/58793583/260b5ee7-151d-4980-8a4c-7161d43bad37)
*Patient Dashboard – View records & appointments.*

![Payment](https://github.com/MrSagarBiswas/E-Health-Management-System/assets/58793583/fb79f1c0-6ade-4866-b50c-a58b25ee6e3b)
*Razorpay Checkout for insurance payments.*

![Chat](https://github.com/MrSagarBiswas/E-Health-Management-System/assets/58793583/ba333ec2-58ee-4e6b-8006-ca723adce959)
*Real-time chat between patient & provider.*

![Records](https://github.com/MrSagarBiswas/E-Health-Management-System/assets/58793583/aa5be4c6-05e4-41ff-a922-a29e6414647b)
*Efficient patient data management with MongoDB.*

---

## License

This project is licensed under the MIT License. See the [LICENSE](https://opensource.org/license/mit) file for details.

---
