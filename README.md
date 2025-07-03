# 🍽️ AI-Powered Restaurant Chatbot

An intelligent restaurant chatbot system built using **Python (Flask)** and **Node.js (Express)**, designed to streamline the dining experience. Customers can place orders, view top-rated items, and receive personalized suggestions — all via a conversational interface.

---

## 📁 Project Structure

restaurantChatbot/ backend/

/server.py # Flask server handling orders and SQLite storage

/index.js # Express.js test API (optional frontend server)

/orders.db # SQLite database storing orders

/orders.json # JSON-based log or backup (optional)

/package.json # Node.js dependencies



## 🚀 Features

- 🧠 **Chat-Based Ordering**: Users can place orders via a chatbot interface.
- 🍱 **Multiple Items & Quantity Support**
- 📝 **Order Notes**: Customizations like *extra spicy* or *no onions*.
- 💾 **Persistent Storage**: Orders saved in SQLite DB.
- 🌐 **Cross-Origin Support**: Flask server allows CORS for frontend integration.
- 🔄 **Node.js Server (Optional)**: A test server for API message response.

---

## ⚙️ Backend Technologies

| Component       | Technology           |
|----------------|----------------------|
| Chat Handling   | Flask (Python)       |
| REST API        | Flask & Express.js   |
| Database        | SQLite               |
| Cross-Origin    | Flask-CORS, CORS     |

---

## 📦 Installation Steps

### 1. Clone the Repo

```bash
git clone https://github.com/yourusername/restaurantChatbot.git

cd restaurantChatbot/backend

### 2. Backend (Python Flask)


# Optional: Create virtual environment

python -m venv venv

source venv/bin/activate  # or venv\\Scripts\\activate on Windows

# Install dependencies
pip install flask flask-cors

# Run Flask server
python server.py

### 3. Node.js Server

If you want to test the Node.js API (index.js):

install node js from https://nodejs.org/en/download

/go to frontend

npm install

npm run dev

📡 API Endpoints
POST /order (Flask)
Place an order.

json

{
  "tableNumber": "T4",
  "items": [
    {"name": "Paneer Butter Masala", "quantity": 2, "price": 150},
    {"name": "Naan", "quantity": 3, "price": 20}
  ],
  "totalCost": 360,
  "note": "Extra spicy"
}

GET /api/message (Express)
Test endpoint — returns: { "message": "Hello from backend!" }

💾 Data Storage
SQLite Database: Stores each order with table number, items, note, and timestamp.

JSON Backup: Orders are optionally logged to orders.json.

📌 To-Do / Future Improvements
✅ Integrate a React frontend chatbot UI

🌤️ Suggest items based on weather

🧾 Add PDF invoice generation

🌍 Multi-language support (e.g., Telugu)

🔐 Admin dashboard for order analytics

🧠 Inspiration
This project is a part of a final-year academic project focusing on intelligent automation in the food industry through AI-powered interaction.

