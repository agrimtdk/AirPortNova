# AirPortNova
# 🛫 AirportNova — PostgreSQL Airport Database System

> ✈️ A full-scale **airport management system** implemented with efficient PostgreSQL schema design.  
> Models real-world airport operations, including flights, airfares, passengers, tickets, and transactions.

---

## 📦 About the Project

AirportNova simulates the backend database of an airport system. It is perfect for educational, enterprise modeling, or backend API/database practice.

### 🔧 Key Features

- 🚀 **Modular schema** with clear normalization
- 🔁 **Realistic relationships**: Airline-Fleet-Flight, Passenger-Ticket-Transaction
- 🧠 **Efficient joinable structure** with bridge tables
- 📌 **Referential integrity** enforced via foreign keys
- 🔎 Designed for scalability and clarity

---

## 🗂️ Entity Overview

| Entity      | Description                                  |
|-------------|----------------------------------------------|
| Country     | Stores country codes and names               |
| City        | City name, state, and associated country     |
| Airport     | Airport code, name, city, and country info   |
| Airline     | Airline ID and name                          |
| Employee    | Personal and contact details of staff        |
| Flight      | Flight info including source, time, duration |
| Passenger   | Passport-wise details of flyers              |
| Ticket      | Travel type, price, source-destination       |
| Airfare     | Fare breakdown per flight                    |
| Route       | Flight path with takeoff and destination     |
| AirplaneType| Aircraft specs like capacity and weight      |
| Transaction | Booking-related transactions and staff       |

---

## 🛠️ Setup Instructions

```bash
git clone https://github.com/yourusername/airportnova.git
cd airportnova
psql -U postgres -f schema.sql
