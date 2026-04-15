# RoyalTable - Dining Table Reservation System

A full-stack dining table reservation system with real-time availability, 20 tables, 15 cities, and 60+ menu items.

## Features
### Frontend

* Animated welcome screen
* 15 Tamil Nadu cities selection
* 3-Star, 4-Star, 5-Star hotel classification
* AC and Non-AC dining option
* Smart meal timing selection
* Date picker (future dates only)
* 20 tables with availability
* Color-coded tables (Available / Reserved)
* OTP verification (Demo: 123456)
* Interactive menu with 60+ items
* Responsive design

### Backend

* RESTful API (6 endpoints)
* SQLite database (auto-created)
* Real-time table availability
* Reservation storage
* Unique booking ID generation
* Pre-reserved tables (3, 7, 12, 15, 18)
* Error handling

### Frontend
* HTML5
* CSS3
* JavaScript (ES6)

### Backend
* Node.js
* Express.js
* SQLite3

### Tools
* Git
* npm
* Nodemon

## Installation

### Prerequisites

* Node.js (v14 or higher)
* npm

### Steps

```bash
git clone https://github.com/YOUR_USERNAME/dining-reservation-system.git
cd dining-reservation-system
npm install
npm start
```

Open browser:
http://localhost:3000

---

## Project Structure

```
dining-reservation/
│
├── package.json
├── database.js
├── server.js
├── reservation.db
├── README.md
├── .gitignore
│
├── public/
│   └── index.html
│
└── node_modules/
```

---

## Usage

1. Select city
2. Choose hotel class
3. Pick hotel
4. Select dining preferences
5. Choose date and number of persons
6. Select table
7. Enter customer details
8. Pay advance (OTP: 123456)
9. View booking summary

---

## API Endpoints

| Method | Endpoint               | Description        |
| ------ | ---------------------- | ------------------ |
| GET    | /api/locations         | Get all cities     |
| GET    | /api/hotels?starClass= | Get hotels         |
| POST   | /api/tables/check      | Check availability |
| POST   | /api/tables/reserve    | Reserve table      |
| POST   | /api/reservations      | Create booking     |
| GET    | /api/reservations/:id  | Get booking        |

---

## Database Schema

### reservations

* id
* location
* star_class
* hotel
* ac_type
* meal_type
* timing
* date
* persons
* table_number
* customer_name
* mobile
* email
* advance_paid
* payment_method

### reserved_tables

* id
* table_number
* date
* hotel

---

## Menu Overview

* 10 Fresh Juices
* 15 Starters
* 20 Veg Main Course
* 20 Non-Veg Main Course
* 20 Desserts

---

## Pre-reserved Tables

Tables 3, 7, 12, 15, 18 are reserved and cannot be selected.

---

## Troubleshooting

### Port already in use

```bash
const PORT = 3001;
```

### Database issues

```bash
del reservation.db   # Windows
rm reservation.db    # Mac/Linux
```

### npm issues

```bash
npm cache clean --force
npm install
```

---

## Contributing

1. Fork the repository
2. Create a branch
3. Commit changes
4. Push to GitHub
5. Create a Pull Request

---

## License

MIT License

---

## Author

Your Name

---

## Support

If you find this project useful, consider giving it a star on GitHub.
