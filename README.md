
# Business Ledger

> **Smart Mobile Ledger Management for Small Businesses & Field Sales Teams**

A comprehensive business ledger, inventory, billing, and customer account management application built with **Flutter** and **SQLite**. Designed for manufacturers, wholesalers, distributors, and small businesses to manage daily sales, collections, invoices, and outstanding balances—completely offline.

<div align="center">

![Flutter](https://img.shields.io/badge/Flutter-3.x-blue?logo=flutter)
![Dart](https://img.shields.io/badge/Dart-3.x-blue?logo=dart)
![SQLite](https://img.shields.io/badge/SQLite-Latest-green?logo=sqlite)
![Firebase](https://img.shields.io/badge/Firebase-Latest-orange?logo=firebase)
![License](https://img.shields.io/badge/License-MIT-green)
![Version](https://img.shields.io/badge/Version-1.0.4-blue)

**A production-ready business management app built from real-world requirements**

</div>

---

## 📖 Table of Contents

- [Demo & Download](#-demo--download)
- [The Problem](#-the-problem)
- [Real-World Application](#-real-world-business-application)
- [Key Features](#-key-features)
- [Why Business Ledger?](#-why-business-ledger)
- [Tech Stack](#-technology-stack)
- [Quick Start](#-quick-start)
- [Project Structure](#-project-structure)
- [Screenshots](#-application-walkthrough)
- [Learning Outcomes](#-learning-outcomes)
- [Future Enhancements](#-planned-enhancements)
- [Use Cases](#-use-cases)
- [Release Info](#-latest-release)
- [Developer](#-developer)

---

## 🎬 Demo & Download

| | |
|---|---|
| **📹 Watch Demo** | [Full Application Walkthrough](https://www.youtube.com/shorts/hJ1GCkaRr_0) |
| **📱 Get APK** | [Download Latest v1.0.4](https://github.com/kritika038/business-ledger/releases/tag/v1.0.4) |

---

## 🚩 The Problem

Sales representatives in wholesale and distribution businesses face significant operational challenges:

- **Manual Errors**: Paper-based ledgers prone to calculation mistakes
- **Data Loss**: No centralized record of transactions
- **Slow Reporting**: Difficulty tracking outstanding balances in real-time
- **Poor Visibility**: Hard to make informed financial decisions on the go
- **Complex Tools**: Desktop accounting software not suited for field operations

**The Need**: A simple, mobile-first solution that works offline and simplifies bookkeeping, billing, and inventory tracking.

---

## 🌍 Real-World Business Application

This project was developed after observing day-to-day operations in a **footwear manufacturing and distribution business**.

The application helps business owners and field sales teams:

- ✅ Track customer balances in real-time
- ✅ Record sales and collections instantly
- ✅ Generate professional invoices on-site
- ✅ Monitor inventory levels
- ✅ Manage complete business operations from a smartphone

**Unlike typical tutorial projects**, this application was designed around **actual business workflows** and operational requirements—solving real problems faced by sales teams and business owners in the field.

---

## ✨ Key Features

### 👥 Customer Management
- Add and edit customer information
- Full customer transaction history
- Advanced customer search
- Outstanding balance tracking per customer

### 💰 Ledger Management
- Record credit and debit transactions
- Automatic running balance calculation
- Real-time outstanding balance visibility
- Complete transaction history

### 🧾 Invoice Management
- Generate professional invoices on-the-go
- Invoice history and customer-wise records
- **PDF export** for easy sharing
- Print-ready invoice formatting

### 📦 Inventory Management
- Real-time product tracking
- Stock level monitoring
- Inventory updates and adjustments
- Available stock visibility

### 📊 Business Intelligence
- **Sales Reports**: Track revenue and performance
- **Outstanding Reports**: Monitor pending payments
- **Collection Reports**: Analyze payment trends
- **Business Reports**: Comprehensive metrics

### 📄 Customer Statement PDFs
- Generate customer-wise statement PDFs
- Running balance calculations
- Professional business format
- Easy sharing and record keeping

### 💬 WhatsApp Sharing
- Share customer statements directly
- Personalized customer messages
- Automatic phone number handling

### 📈 Collection Breakdown
- Cash Collection Tracking
- UPI Collection Tracking
- Bank Collection Tracking
- Dashboard level visibility

### 💳 Payment Tracking
- Record collections instantly
- Track pending and overdue payments
- Payment history by customer
- Collection performance metrics

### 🛡️ Data Management
- **Local Backup**: Secure on-device backups
- **Restore Functionality**: Recover business records
- **PDF Exports**: Generate shareable reports
- **Offline-First**: Works without internet

---

## 🎯 Why Business Ledger?

| Feature | Benefit |
|---------|---------|
| **Mobile-First** | Manage business from anywhere, anytime |
| **Completely Offline** | No internet required—SQLite local database |
| **Instant Visibility** | Real-time outstanding balance tracking |
| **Fast & Simple** | Easy workflows designed for field teams |
| **Professional Output** | Generate invoices and reports on-device |
| **Secure & Local** | All data stays on your phone |
| **Zero Subscription** | One-time download, permanent access |

---

## 🏗️ Technology Stack

```
Frontend:              Flutter, Dart
Database:              SQLite (sqflite)
State Management:      Provider
Cloud Services:        Firebase Authentication
Backup & Sync:         Firestore
PDF Generation:        PDF, Printing Packages
Sharing:               Share Plus, URL Launcher
Local Storage:         Shared Preferences
Development Tools:     Android Studio, VS Code, Git
```

---

## 🚀 Quick Start

### Prerequisites
- Flutter SDK installed
- Android Studio or VS Code
- Git

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/kritika038/business-ledger.git
   cd business-ledger
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Run the application**
   ```bash
   flutter run
   ```

---

## 📁 Project Structure

```
lib/
├── models/              # Data models
├── screens/             # UI screens
├── widgets/             # Reusable widgets
├── services/            # Business logic
├── database/            # SQLite operations
├── providers/           # State management
├── utils/               # Helper functions
└── main.dart            # Entry point
```

---

## 📸 Application Walkthrough

| Feature | Screenshot |
|---------|-----------|
| Dashboard Overview | ![Dashboard](screenshots/01_dashboard_overview.jpeg) |
| Pending Payments | ![Pending Payments](screenshots/02_pending_payments_dashboard.jpeg) |
| Transaction History | ![Transactions](screenshots/03_transaction_history.jpeg) |
| Invoice Management | ![Invoices](screenshots/04_invoice_management.jpeg) |
| Inventory Tracking | ![Inventory](screenshots/05_inventory_management.jpeg) |
| Business Reports | ![Reports](screenshots/06_business_reports.jpeg) |

---

## 📚 Learning Outcomes

This project provided hands-on experience with:

- **Mobile Development**: Flutter & Dart best practices
- **Database Design**: SQLite architecture and optimization
- **State Management**: Provider pattern implementation
- **PDF Generation**: On-device invoice and report creation
- **UI/UX Design**: Mobile-first user experience
- **Business Logic**: Real-world accounting workflows
- **Version Control**: Git & GitHub collaboration

---

## 🔮 Planned Enhancements

- ☁️ Firebase Cloud Sync
- 👥 Multi-user Account Support
- 🧾 GST-compliant Billing
- 📱 Barcode Scanning Integration
- 💬 WhatsApp Invoice Sharing
- 📊 Advanced Analytics Dashboard
- 🏢 Multi-Business Management
- 🌐 Cloud Backup & Restore

---

## 📋 Use Cases

Perfect for:
- **Manufacturers** managing wholesale orders
- **Distributors** tracking retailer accounts
- **Field Sales Teams** collecting payments on-site
- **Small Businesses** with simple accounting needs
- **Wholesalers** managing outstanding receivables
- **Inventory-Heavy Businesses** monitoring stock levels

---

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report issues
- Suggest features
- Submit pull requests

---

## 📄 License

This project is available on GitHub. Check the repository for license details.

---

## 📦 Latest Release

**Version:** 1.0.4  
**Build:** 5

📥 **[Download APK](https://github.com/kritika038/business-ledger/releases/tag/v1.0.4)**

---

## 👩‍💻 Developer

**Kritika Bansal**  
B.Tech Computer Science (Artificial Intelligence)

- 🔗 [GitHub](https://github.com/kritika038)
- 📱 [Project Repository](https://github.com/kritika038/business-ledger)

---

## ⭐ Show Your Support

If this project helped you, please consider giving it a **star** on GitHub—it helps others discover it!

---

<div align="center">

**Built with ❤️ for small businesses and field sales teams**

[⬆ Back to Top](#business-ledger)

</div>
