
# 🎁 Gift Guru – AI-Powered Gift Recommendation App

Gift Guru is an AI-powered gift recommendation system built using **React (Vite)** for the frontend and **Node.js (Express)** for the backend.
It uses **Google Gemini API** to generate personalized product recommendations and displays them beautifully with product, descriptions, and direct buy links.

---

## 🚀 Features

### 🧠 AI-Based Recommendations

* Uses **Google Gemini** to analyze recipient details (age, interests, relation, budget).
* Generates **smart and personalized** gift suggestions.

### 🎨 Stunning Frontend (React + TailwindCSS)

* Clean and modern UI
* Fully responsive
* Attractive gift cards with name, price, description & Buy Now link

### 🔗 Working Product Links

Each recommendation includes:

* Product Name
* Description
* Approx Price
* Buy Now Link

### ⚡ Fast Backend (Node.js + Express)

* Connects securely with Gemini API
* Ensures clean response structure for frontend
* Validates user input

---

## 📂 Folder Structure

```
gift-guru/
│
├── backend/
│   ├── server.js
│   ├── package.json
│   ├── .env
│   └── node_modules/
│
└── frontend/
    ├── index.html
    ├── package.json
    ├── vite.config.js
    ├── tailwind.config.js
    ├── postcss.config.js
    └── src/
        ├── main.jsx
        ├── App.jsx
        ├── index.css
        └── components/
            ├── GiftForm.jsx
            └── RecommendationCard.jsx
```

---

## 🛠️ Installation & Setup

### 🔹 1. Clone the Repository

```
git clone https://github.com/<your-username>/<your-repo>.git
cd gift-guru
```

---

# 🖥️ Backend Setup

### 🔹 2. Go to the backend folder

```
cd backend
```

### 🔹 3. Install dependencies

```
npm install
```

### 🔹 4. Create `.env` file

```
GOOGLE_API_KEY=your_api_key_here
```

Make sure ✔ **no quotes**, ✔ **no spaces**.

### 🔹 5. Start backend

```
node server.js
```

Backend runs at:

👉 `http://localhost:5000/api/recommend`

---

# 🌐 Frontend Setup

### 🔹 1. Go to frontend folder

```
cd frontend
```

### 🔹 2. Install dependencies

```
npm install
```

### 🔹 3. Start the frontend

```
npm run dev
```

Open in browser:
👉 [http://localhost:5173](http://localhost:5173)

---

## 🧪 API Testing (Postman)

Send **POST** request:

```
http://localhost:5000/api/recommend
```

**Raw JSON Body:**

```json
{
  "age": 25,
  "relationship": "Friend",
  "interests": "technology, gadgets",
  "budget": "2000-5000"
}
```

---

## ✔ Output JSON Format

Example:

```json
{
  "success": true,
  "recommendations": [
    {
      "title": "Echo Dot (5th Gen)",
      "description": "A smart speaker with Alexa...",
      "price": "₹4,499",
      "image": "https://example.com/image.jpg",
      "link": "https://amazon.in/example"
    }
  ]
}
```

---

# 🚨 Common Fixes

### ❌ API key invalid error

✔ Ensure `.env` exists
✔ Restart backend
✔ Use correct model:

```
gemini-1.5-flash
```

### ❌ Images not loading

✔ Ensure your AI prompt outputs **valid HTTPS images only**

### ❌ Buy Now link broken

✔ Always validate URL format in the backend

---

## 📸 Screenshots

(Add UI screenshots here optionally)

---

# 🤝 Contributing

Pull requests are welcome.
For major changes, please open an issue first.

---

# 📜 License

This project is licensed under the **MIT License**.


