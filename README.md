# The-Montessa-Restaurant-
Overview
The Montess Restaurant Management System is a full-stack application designed to streamline restaurant ordering and management processes.
It allows users to register, log in, browse menu items, add items to cart, place orders, and make payments, while the admin has full control over menu, users, and orders.
- This system integrates Firebase (for authentication and real-time updates) and MongoDB (for storing structured data such as users, orders, and menu items).
- npm run dev used for restaurent-client
- npm start for the restaurent-backend  
  
⚙️ Features
👤 User Module
- User registration and login (via Firebase Authentication).
- View and browse food menu with categories.
- Add items to cart and manage quantities.
- Checkout and complete payment securely.
- View past orders and order history.

Admin Module:-
- Admin login with special privileges.
- Manage menu items (add, edit, delete dishes).
- View and manage all user accounts and orders.
- Track order status and update delivery progress.
- Access full database control (via Firebase + MongoDB).
  
 System Architecture:- 
- The application follows a modular MVC structure:

- Frontend: Built using React.js / HTML / CSS for interactive UI.

- Backend: Node.js + Express.js for API handling.

- Database: Firebase (Authentication + Realtime updates), MongoDB (menu, orders, cart data).

Database Structure
Firebase
Used for:
- Authentication (User login/signup)
- Realtime status updates
- Cloud messaging (optional notifications)
  
MongoDB
Collections:

users
{
  "userId": "auto-generated",
  "name": "John Doe",
  "email": "john@example.com",
  "role": "user",
  "cart": []
}


menu
{
  "itemId": "auto-generated",
  "name": "Cheese Pizza",
  "price": 250,
  "category": "Pizza",
  "description": "Freshly baked with mozzarella",
  "imageURL": "link_to_image"
}

Payment Module:-
Integrated with a payment gateway (e.g., Stripe / Razorpay).
Users can pay via debit/credit card or UPI.
Payment confirmation updates both Firebase and MongoDB databases.

