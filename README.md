# 🏨 Grand Aurelia — Hotel Management System

A fully client-side hotel management web app built with vanilla HTML, CSS, and JavaScript.
Designed for both hotel staff and guests, featuring a QR-based authentication system,
live order management, and printable room access cards.

## ✨ Features

### 🔐 Guest Login Portal
- **QR Code Login** — Live camera scanner reads room card QR codes and verifies a
  secure token for instant authentication
- **Manual Login** — Room number + guest name as password, validated against the registry
- Demo mode to simulate QR login without a physical card

### 🪪 QR Card Generator (Staff)
- Fill in guest details to generate a unique token string encoded as a QR code
- Token format: `AURELIA|ROOM|NAME|SECURETOKEN`
- Preview, print, or download the room access card
- One-click guest registration activates the room in the live system

### 👔 Staff Dashboard
- Live overview of occupied rooms, pending orders, service requests, and staff calls
- Confirm and mark food orders as delivered
- Complete room service and amenity requests
- Visual room status grid (Vacant / Occupied / Service Pending / Staff Called)

### 🛎️ Guest Services
- **Order Food** — Full dining menu with categories, quantity controls, and a cart
- **Room Service** — Request housekeeping, towels, massage, laundry, and more
- **Pay Bill** — Itemised statement with multiple payment methods (Card, UPI, Cash, Net Banking)
- **Call Staff** — Animated bell with request type and optional notes
- **My Orders** — Real-time order and request tracking

## 🛠 Tech Stack
- Pure HTML5, CSS3, JavaScript (no frameworks)
- [QRCode.js](https://github.com/davidshimjs/qrcodejs) — QR code generation
- [jsQR](https://github.com/cozmo/jsQR) — In-browser QR code scanning via camera
- Google Fonts (Cormorant Garamond + Jost)

## 🚀 Usage
No build step or server required. Just open `hotel-management.html` in any modern browser.

> **Staff Portal** → Generate QR cards, manage orders, monitor rooms  
> **Guest Portal** → Scan QR or login manually → access all room services
