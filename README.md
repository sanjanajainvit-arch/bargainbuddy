# 🛒 PriceWise - E-Commerce Price Tracking & Alert System

<p align="center">
  <img src="https://img.shields.io/badge/Next.js-Framework-black" />
  <img src="https://img.shields.io/badge/MongoDB-Database-green" />
  <img src="https://img.shields.io/badge/TypeScript-Language-blue" />
  <img src="https://img.shields.io/badge/Cheerio-Web%20Scraping-orange" />
  <img src="https://img.shields.io/badge/Nodemailer-Email-red" />
</p>

## 📌 Overview

PriceWise is a full-stack e-commerce price monitoring platform that automatically tracks product prices from online marketplaces and notifies users whenever significant price changes occur.

The application continuously scrapes product information, stores historical price data, analyzes trends, and sends automated email alerts for price drops, stock availability, and discount opportunities.

---

## 🚀 Features

### 🔍 Product Tracking

* Track products using product URLs
* Monitor current and historical prices
* Store complete pricing history

### 📊 Price Analytics

* Lowest Price Detection
* Highest Price Tracking
* Average Price Calculation
* Discount Percentage Monitoring

### 📧 Automated Notifications

* Welcome Email
* Lowest Price Alert
* Product Restocked Alert
* Discount Threshold Alert

### ⏰ Scheduled Monitoring

* Automated Cron Jobs
* Periodic Product Re-Scraping
* Database Updates
* Smart Notification Triggers

### 🎨 User Interface

* Responsive Design
* Product Dashboard
* Product Details Page
* Modern UI with Tailwind CSS

---

## 🏗️ System Architecture

```text
User
 │
 ▼
Frontend (Next.js + Tailwind CSS)
 │
 ▼
API Layer
 │
 ▼
Web Scraper (Axios + Cheerio)
 │
 ▼
MongoDB Database
 │
 ▼
Price Analysis Engine
 │
 ▼
Email Notification Service
 │
 ▼
User Inbox
```

---

## 🛠️ Tech Stack

### Frontend

* Next.js
* React
* Tailwind CSS
* Headless UI

### Backend

* Node.js
* TypeScript
* Next.js Server Actions

### Database

* MongoDB
* Mongoose

### Web Scraping

* Axios
* Cheerio
* Bright Data Proxy

### Notifications

* Nodemailer
* SMTP Email Service

### Automation

* Cron Jobs

---

## 📂 Project Structure

```text
PriceWise/
│
├── app/
├── components/
├── lib/
│   ├── scraper/
│   ├── models/
│   ├── mongoose/
│   ├── nodemailer/
│   └── utils/
│
├── public/
├── styles/
├── types/
│
├── .env
├── next.config.js
├── tailwind.config.ts
├── package.json
└── README.md
```

---

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/pricewise.git
cd pricewise
```

### Install Dependencies

```bash
npm install
```

---

## 🔐 Environment Variables

Create a `.env` file in the root directory:

```env
# Bright Data Credentials
BRIGHT_DATA_USERNAME=
BRIGHT_DATA_PASSWORD=

# MongoDB Database
MONGODB_URI=

# Email Configuration
EMAIL_USER=
EMAIL_PASS=
```

---

## ▶️ Running the Application

Start the development server:

```bash
npm run dev
```

Open:

```text
http://localhost:3000
```

---

## 🔄 Application Workflow

### Step 1: Product Submission

User enters an e-commerce product URL.

### Step 2: Data Extraction

The scraper extracts:

* Product Title
* Current Price
* Original Price
* Product Images
* Availability Status
* Discount Percentage

### Step 3: Data Storage

Product information is stored in MongoDB.

### Step 4: Automated Monitoring

Cron jobs periodically:

* Re-scrape products
* Compare pricing data
* Update price history

### Step 5: Alert Generation

Users receive email notifications when:

* Product reaches lowest recorded price
* Product is back in stock
* Discount threshold is reached

---

## 📈 Sample Use Cases

### 🛍️ Consumers

Track products and purchase them at the best possible price.

### 🏪 Sellers

Monitor competitor pricing strategies.

### 📊 Market Research

Analyze product pricing trends over time.

---

## 🎯 Key Learning Outcomes

This project helped strengthen skills in:

* Full Stack Development
* Web Scraping Techniques
* Database Design
* API Development
* Email Automation
* TypeScript Development
* Cron Job Scheduling
* Production Application Architecture

---

## 📸 Screenshots

Add your screenshots here:

```text
screenshots/homepage.png
screenshots/product-details.png
screenshots/email-alert.png
```

Example:

```md
![Homepage](screenshots/homepage.png)
![Product Details](screenshots/product-details.png)
![Email Alert](screenshots/email-alert.png)
```

---

## 🔮 Future Enhancements

* AI-Based Price Prediction
* User Authentication
* Personalized Watchlists
* Multi-Vendor Product Tracking
* Advanced Analytics Dashboard
* Mobile Application Support

