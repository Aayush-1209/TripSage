# TripSage - Destination Recommendation App

## 🌍 Introduction
TripSage is a **full-stack travel recommendation platform** that personalizes destination suggestions based on user preferences. Users can explore destinations, plan itineraries, and leave reviews, while admins manage destinations and reviews efficiently.

## 🏗️ Project Type
**Fullstack Application** (Frontend + Backend)

## 🚀 Deployed App
- **Frontend:** [Frontend Live URL](https://tripsage.netlify.app/)
- **Backend:** [Backend Live URL](https://tripsage.onrender.com)
- **Database:** MongoDB Atlas

## 📁 Directory Structure
```
TripSage/
├─ backend/
│  ├─ controllers/
│  ├─ models/
│  ├─ routes/
│  ├─ config/
│  ├─ server.js
├─ frontend/
│  ├─ src/
│  │  ├─ components/
│  │  ├─ pages/
│  │  ├─ context/
│  │  ├─ App.js
│  ├─ public/
│  ├─ index.js
```

## 📽️ Video Walkthrough
**Project Walkthrough:** [https://youtu.be/tbjPRjz-eOA]

**Codebase Walkthrough:** [https://youtu.be/tbjPRjz-eOA]

## 🌟 Features
✅ **User Features:**  
- Personalized destination recommendations
- Search, filter, and sort destinations
- Plan trips with custom itineraries
- Leave and view reviews on destinations

✅ **Admin Features:**  
- Manage (Add/Edit/Delete) destinations
- View and delete reviews

## 🎨 Home Page Preview
**![Screenshot 2025-03-25 114247](https://github.com/user-attachments/assets/18d3cbc0-e630-4079-a2ac-c4c684a2c59a)
**

## 🗺️ Destinations Page Preview
** ![Screenshot 2025-03-25 115747](https://github.com/user-attachments/assets/4340459c-f5ee-4a30-af15-a3c1d6e4bb56)
           **

## 🛠️ Admin Dashboard Preview
** ![Screenshot 2025-03-25 115916](https://github.com/user-attachments/assets/d25e9614-8bdb-4e31-b216-0ae32287c524)
     **

## 🎯 Design Decisions & Assumptions
- **User Preferences Stored in User Schema:** Eliminated the separate `preferences` model to simplify querying and reduce database complexity.
- **Role-Based Access Control:** Admins have full control over destinations and reviews, while users can only manage itineraries and preferences.
- **Optimized Queries:** Used indexing and aggregation for efficient data retrieval.

## 🛠️ Installation & Getting Started
Clone the repository and install dependencies:
```bash
# Backend Setup
cd backend
npm install
npm start

# Frontend Setup
cd frontend
npm install
npm run dev
```

## 🏆 Usage
### **For Users:**
1. **Signup/Login** to access personalized recommendations.
2. **Browse destinations** and use filters.
3. **Plan a trip** by adding itineraries.
4. **Leave reviews** for destinations.

### **For Admins:**
1. **Login with admin credentials**.
2. **Manage destinations** (Add/Edit/Delete).
3. **View and delete user reviews**.

## 🔑 Credentials
**Admin Login:**  
- Email: `aayush@example.com`  
- Password: `123456`  

**Test User Login:**  
- Email: `aayush.user@gmail.com`  
- Password: `12345`  

## 🌍 APIs Used
- JWT (for secure authentication)

## 🔥 API Endpoints
### **User Authentication**
- `POST /signup` - Register a new user
- `POST /login` - Authenticate user

### **Destinations**
- `GET /destinations/` - Retrieve all destinations
- `POST /destinations/create` - Add new destination (Admin)
- `DELETE /destinations/delete/:id` - Remove a destination (Admin)

### **Itineraries**
- `POST /itineraries/add` - Add a new itinerary
- `GET /itineraries/user` - Fetch user-specific itineraries
- `DELETE /itineraries/delete/:id` - Delete an itinerary

### **Reviews**
- `POST /reviews/add` - Add a new review
- `DELETE /reviews/delete/:id` - Delete a review (Admin)

## 💡 Technology Stack
- **Frontend:** React.js, Tailwind CSS, React Router
- **Backend:** Node.js, Express.js, MongoDB
- **Authentication:** JWT (JSON Web Token)
- **Deployment:** Netlify (Frontend), Render (Backend)

---
🙌 **Thanks for checking out TripSage!** Feel free to contribute or reach out for any queries! 🚀


