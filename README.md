from pathlib import Path

readme_content = """
# 🍽️ EatPlus

**EatPlus** is a digital restaurant ordering platform that allows diners to scan table-specific QR codes, browse dynamic menus, place orders, and pay — all from their phones. Restaurant owners can manage menus, view orders, and access feedback through a live dashboard.

---

## 🧩 Problem Statement

Restaurants struggle with:
- Outdated paper menus
- Inefficient order handling
- Delayed billing and feedback collection

---

## 🎯 Objective

To build a system that digitizes dine-in experiences by:
- Offering QR-based table menus
- Enabling instant order placement and tracking
- Allowing staff to manage kitchen workflows efficiently

---

## ✅ Solution

EatPlus provides:
- Microsites for every restaurant: `eatplus.com/<slug>`
- Real-time menu and order updates using Firebase
- React dashboard for both diners and restaurant staff
- Payment integrations via Razorpay/Stripe

---

## 🚀 Features

- 👤 Diner: Scan → Order → Pay → Review
- 👨‍🍳 Owner: Register → Manage Menu → Monitor Orders
- 🧾 Staff: Live Kitchen Console (NEW → READY → SERVED)
- 🔐 Auth via Firebase (DINER, OWNER, STAFF roles)
- 📦 Hosted on Firebase (Frontend) and Render/GCP (Backend)

---

## 🛠 Tech Stack

- **Frontend**: React (JSX), Vite, Tailwind
- **Backend**: FastAPI (Python)
- **Database**: Firebase Firestore
- **Auth/Storage**: Firebase Auth & Storage
- **Payments**: Razorpay / Stripe

---

## 📥 Getting Started

1. Clone the repo
2. Setup Firebase project
3. Start frontend: `npm run dev`
4. Start backend: `uvicorn main:app --reload`

---

> Designed for modern restaurants to deliver a smarter dining experience.
"""

readme_path = Path("README.md")
readme_path.write_text(readme_content)
