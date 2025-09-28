

# RJCouriers — Reference Manual

> **Project type:** MERN (MongoDB, Express, React, Node.js) — includes both a monolithic version and a microservice version.

---

## 1. Overview
RJCouriers is a package delivery website built with a menu-driven interface. The project demonstrates two designs:
- **Monolithic:** Single application containing frontend + backend + database.
- **Microservices:** Separate small services (Auth, Orders, Tracking, etc.) connected via API Gateway.

---

## 2. Tech Stack
- **Frontend:** React (menu-driven UI)
- **Backend:** Node.js + Express
- **Database:** MongoDB (Mongoose)
- **Auth:** JWT

---

##  Sample Image ScreenShot
<img width="1273" height="724" alt="image" src="https://github.com/user-attachments/assets/e0e0994d-19d6-4f77-9a5b-7a9790f94629" />

<img width="1275" height="588" alt="image" src="https://github.com/user-attachments/assets/9557a387-6574-4020-a79f-4ffad0e75181" />

<img width="1297" height="594" alt="image" src="https://github.com/user-attachments/assets/4a847bfe-62ed-4089-ab29-b5457df0f235" />

## 3. Setup & Run
### Monolithic App
1. Clone repo → `cd rjcouriers-monolith`
2. Install dependencies in `server` and `client`.
3. Create `.env` with:
```
PORT=5000
MONGO_URI=mongodb://localhost:27017/rjcouriers
JWT_SECRET=secret
```
4. Start: `npm run dev`
5. Open: `http://localhost:3000`

### Microservices App
1. Clone repo → `cd rjcouriers-microservices`
2. Install dependencies for each service (`auth`, `orders`, `tracking`, `gateway`, `ui`).
3. Create `.env` for each service (PORT, MONGO_URI, JWT_SECRET).
4. Run services individually or with Docker Compose.
5. Open UI: `http://localhost:3000`

---

## 4. Main Features
- **Customer:** Place order, track order, view profile.
- **Courier:** View assigned orders, update status/location.
- **Admin:** Manage users, orders, and couriers.

---

## 5. API Endpoints (Examples)
- `POST /api/auth/register` — Register user
- `POST /api/auth/login` — Login & get JWT
- `POST /api/orders` — Place new order
- `GET /api/tracking/order/:id` — Track an order

---

## 6. Submission Checklist
- [x] Both apps run locally
- [x] Screenshots added in `docs/screenshots/`
- [x] Repo uploaded to GitHub with README

---

**Note:** Keep `.env` files private and only share `.env.sample` for reference.

