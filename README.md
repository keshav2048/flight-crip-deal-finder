# ✈️ FlightCrip – Automated Flight Deal Tracker

FlightCrip is a Python-based automation tool that tracks flight prices and sends notifications via **SMS and email** when deals drop below your specified budget. Perfect for travelers who want to save time and money by letting the code do the searching!

---

## 🚀 Features

- 🧾 Pulls destination and price data from a **Google Sheet** using the Sheety API
- 🔎 Fetches flight data using the **amadeus API** 
- 📩 Sends **email alerts** using Python’s `smtplib`
- 📱 Sends **SMS notifications** using the **Twilio API**
- 📋 Users register through a **Google Form** and are automatically added to the notification list
- 📊 Real-time price comparison and alerting for cheapest flights

---

## 🛠️ Tech Stack

- **Python 3**
- **APIs:**  
  - [Sheety API](https://sheety.co/) – for Google Sheets integration  
  - [Amadeus API](https://tequila.kiwi.com/) – for flight search  
  - [Twilio API](https://www.twilio.com/) – for SMS notifications  
- **Libraries:** `requests`, `smtplib`, `datetime`

---

## 📂 Project Structure

```bash
flight-crip-deal-finder/
│
├── data_manager.py           # Handles reading/writing to Google Sheets
├── flight_data.py            # Stores and structures flight search results
├── flight_search.py          # Handles calls to the Tequila API
├── notification_manager.py   # Sends SMS and email alerts
├── main.py                   # Orchestrates everything
├── requirements.txt          # Python dependencies
└── .env.example              # Template for API keys (DO NOT commit real secrets)
