# Electricity-Board
A responsive electricity meter &amp; bill management web app with local storage, bill generation, sharing, and PWA support.

# ⚡ Lavanya Singh Electricity Board

A responsive, browser-based electricity meter and personal bill management application built with **HTML, CSS, and JavaScript**.

The application helps users manage consumer profiles, record monthly meter readings, calculate electricity consumption, maintain reading history, and generate a downloadable/shareable bill preview.

> **Note:** This is a personal electricity record application and **not an official electricity utility billing system**.

## ✨ Features

* 👤 Create and manage multiple consumer profiles
* 🔢 Store consumer and meter numbers
* 🏠 Save consumer address details
* 📅 Record monthly meter readings
* ⚡ Automatically calculate monthly consumption
* 💰 Electricity charge calculation at ₹5 per unit
* 📊 View monthly reading history
* 📷 Upload an optional meter photo
* 🧾 Generate a professional bill preview
* ⬇️ Download the bill as a PNG image
* 📤 Share the bill directly from supported mobile browsers
* 💾 Store records using browser `localStorage`
* 📱 Responsive design for mobile and desktop
* 📲 PWA installation support
* 🔒 Records remain stored locally in the browser

## 🛠️ Tech Stack

* **HTML5** – Application structure
* **CSS3** – Responsive UI and styling
* **JavaScript** – Application logic and calculations
* **LocalStorage** – Local data persistence
* **Canvas API** – Bill image generation
* **FileReader API** – Meter photo handling
* **Web Share API** – Bill sharing
* **Service Worker** – PWA support

## 📋 How It Works

### 1. Consumer Profile

Create or select a consumer by entering:

* Consumer Name
* Consumer Number
* Address
* Meter Number

The profile is saved locally in the browser.

### 2. Monthly Meter Reading

Enter:

* Billing Month
* Current Meter Unit
* Previous Meter Unit
* Optional Meter Photo

The application calculates consumption using:

```text
Monthly Consumption = Current Reading - Previous Reading
```

### 3. Bill Calculation

The current version uses a fixed rate of **₹5 per unit**.

```text
Energy Charge = Units Consumed × ₹5
```

For example:

```text
Current Reading  = 1250
Previous Reading = 1200

Consumption = 1250 - 1200
            = 50 units

Bill Amount = 50 × ₹5
            = ₹250
```

### 4. Bill Preview

The application generates a bill image containing:

* Consumer details
* Meter details
* Billing month
* Previous and current readings
* Monthly consumption
* Energy charges
* Meter photo
* Total amount
* Record information

### 5. Save & Share

The generated bill can be:

* Downloaded as a PNG image
* Shared directly on supported mobile browsers

## 💾 Data Storage

Consumer profiles and monthly readings are stored using browser `localStorage`.

This means:

* No external database is required
* No backend server is required
* Data stays in the browser on the current device
* Clearing browser storage can remove saved records

## 📱 PWA Support

The project includes Progressive Web App functionality with:

* Web App Manifest
* Install App button
* Service Worker registration
* Mobile installation support

On supported browsers, the application can be installed and used like a mobile application.

## 📂 Project Structure

```text
project/
│
├── index.html
├── lavanya-eb.webmanifest
├── service-worker.js
└── lseb-icon.svg
```

> Make sure the manifest, service worker, and icon files are placed in the correct location for PWA features to work properly.

## 🚀 Getting Started

### Run Locally

1. Clone the repository:

```bash
git clone https://github.com/your-username/lavanya-singh-electricity-board.git
```

2. Open the project folder.

3. Run `index.html` in a modern web browser.

For full PWA functionality, serve the project through an **HTTPS-enabled web server**.

## 📸 Application Flow

```text
Consumer Profile
       ↓
Monthly Meter Reading
       ↓
Consumption Calculation
       ↓
Reading History
       ↓
Bill Preview
       ↓
Download / Share
```

## ⚠️ Disclaimer

This application is designed for **personal electricity record keeping and demonstration purposes**.

It does not represent an official electricity board, utility provider, or government billing system.

The electricity rate and billing rules used in the application are simplified and should not be considered an actual utility tariff.

## 🔮 Future Improvements

Possible future enhancements include:

* Backend database integration
* User authentication
* Real electricity tariff slabs
* Automatic PDF bill generation
* Cloud backup and synchronization
* Multiple tariff plans
* Payment integration
* Advanced consumption charts
* Dark mode
* Admin dashboard
* Official utility API integration

## 👨‍💻 Author

**Lavanya Singh**

Built as a personal electricity record and bill management web application.

---

⭐ If you find this project useful, consider giving the repository a star!
