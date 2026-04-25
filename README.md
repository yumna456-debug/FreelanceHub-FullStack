# FreelanceHub — Full-Stack Freelance Marketplace

A complete full-stack web application built with **HTML/CSS/JavaScript** (frontend) and **Node.js + Express.js** (backend), simulating a freelance services marketplace like Fiverr.



## 🚀 Features

### Frontend
- **Home Page** — Hero section, category chips, featured services
- **Services Listing** — Full service catalog with search, filter, sort
- **Service Detail Modal** — Full details popup for each service
- **Hire Modal** — Confirmation dialog with optional message to seller
- **User Dashboard** — Saved services, hired orders, spending stats
- **Drag & Drop** — Drag service cards to Save or Hire drop zones
- **Responsive Design** — Mobile-first, works on all screen sizes
- **Toast Notifications** — Animated feedback messages

### Backend (Express.js)
- RESTful API with proper status codes (200, 201, 404, 409, 500)
- Request validation and error handling middleware
- In-memory data storage for saved/hired services
- CORS enabled for frontend-backend communication

---

## 📁 Project Structure

```
FreelanceHub/
├── client/
│   ├── index.html          # Main HTML (all pages)
│   ├── css/
│   │   └── style.css       # All styles (Flexbox, Grid, Variables)
│   └── js/
│       └── app.js          # All frontend logic (fetch, DOM, drag-drop)
├── server/
│   ├── server.js           # Express app entry point
│   ├── routes/
│   │   └── services.js     # All API route definitions
│   ├── controllers/
│   │   └── servicesController.js  # Route logic
│   └── data/
│       └── services.js     # In-memory service data (12 services)
├── package.json
└── README.md
```

---

## 🔌 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/services` | Get all services (supports `?search=`, `?category=`, `?sort=`, `?maxPrice=`, `?minRating=`) |
| GET | `/api/services/:id` | Get a single service by ID |
| POST | `/api/services` | Add a new service |
| POST | `/api/save` | Save a service (body: `{ serviceId }`) |
| POST | `/api/hire` | Hire a service (body: `{ serviceId, message }`) |
| GET | `/api/saved` | Get all saved services |
| GET | `/api/hired` | Get all hired orders |
| DELETE | `/api/saved/:id` | Remove a service from saved |

---

## ⚙️ Setup Instructions

### Prerequisites
- [Node.js](https://nodejs.org/) (version 14 or higher)
- npm (comes with Node.js)



### Step 4 — Open in Browser
Visit: **http://localhost:3000**



---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | HTML5, CSS3, Vanilla JavaScript |
| Backend | Node.js, Express.js |
| Data | In-memory arrays (no database needed) |
| Fonts | Google Fonts (Syne + DM Sans) |

---


