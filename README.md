# Kritika Business Ledger

[![Build Status](https://img.shields.io/badge/Build-Success-success.svg?style=for-the-badge&logo=android)](https://github.com/kritika038/kritika-business-ledger-showcase)
[![Platform](https://img.shields.io/badge/Platform-Android-007ACC.svg?style=for-the-badge&logo=android)](https://github.com/kritika038/kritika-business-ledger-showcase)
[![Framework](https://img.shields.io/badge/Framework-Flutter-02569B.svg?style=for-the-badge&logo=flutter)](https://github.com/kritika038/kritika-business-ledger-showcase)
[![Language](https://img.shields.io/badge/Language-Dart-0175C2.svg?style=for-the-badge&logo=dart)](https://github.com/kritika038/kritika-business-ledger-showcase)
[![Database](https://img.shields.io/badge/Database-SQLite-003B57.svg?style=for-the-badge&logo=sqlite)](https://github.com/kritika038/kritika-business-ledger-showcase)
[![Auth](https://img.shields.io/badge/Auth-Firebase-FFCA28.svg?style=for-the-badge&logo=firebase)](https://github.com/kritika038/kritika-business-ledger-showcase)
<br/>
[![Stars](https://img.shields.io/github/stars/kritika038/kritika-business-ledger-showcase?style=for-the-badge)](https://github.com/kritika038/kritika-business-ledger-showcase/stargazers)
[![Forks](https://img.shields.io/github/forks/kritika038/kritika-business-ledger-showcase?style=for-the-badge)](https://github.com/kritika038/kritika-business-ledger-showcase/network/members)
[![Last Commit](https://img.shields.io/github/last-commit/kritika038/kritika-business-ledger-showcase?style=for-the-badge)](https://github.com/kritika038/kritika-business-ledger-showcase/commits/main)

**Kritika Business Ledger** is a mobile-first business management application designed to track sales, simplify collection recording, monitor outstanding balances, and generate professional PDF invoices directly from mobile devices. It is built as a fast, reliable, and offline-first solution for on-the-field operations.

---

## 📋 Project Overview
Kritika Business Ledger streamlines daily billing, ledger management, collections, and customer account tracking for manufacturing, wholesale, and distribution businesses. By prioritizing mobile user interfaces and local storage efficiency, the application ensures that transactions can be recorded and balanced instantly, even in areas with limited internet connectivity.

### Problem Statement
This project was inspired by real challenges observed in a footwear manufacturing and distribution business. Managing field operations requires sales agents and business owners to track daily sales, record payment collections, and monitor customer outstanding balances directly while visiting merchant stores. 

Traditional bookkeeping methods rely on paper logbooks, which are highly prone to calculation errors and offer zero real-time visibility. On the other hand, enterprise desktop accounting packages are overly complex for daily operational workflows and completely inaccessible during field visits. The business needed a mobile-first, simple bookkeeping ledger optimized for rapid on-site entry, balance validation, and instant invoice dispatch.

### Why It Was Built
* **Real-time receivables visibility**: Instant monitoring of outstanding client balances to expedite collections.
* **On-the-go billing**: Ability to create and share customer invoices during deliveries.
* **Offline resilience**: Complete operational independence in warehouses and remote markets.
* **Operational simplicity**: Simplified mobile flows that replace complex bookkeeping ledger journals.

## 🎯 Real-World Impact
This application was developed after observing day-to-day operational challenges in a footwear manufacturing and distribution business.

The solution replaces manual ledger books and reduces dependency on desktop-centric accounting workflows by providing:
- Mobile-first customer ledger management
- Instant outstanding balance visibility
- Faster sales and collection entry
- Professional PDF invoice generation
- Offline business operations

The application is designed around real business workflows rather than tutorial or demonstration scenarios.

---

## 🛠️ Technology Stack
* **Frontend Framework**: Flutter (Dart)
* **UI Design System**: Material 3 UI
* **Authentication Services**: Firebase Core, Firebase Authentication, Google Sign-In API
* **Local Persistence**: SQLite (via `sqflite` plugin)
* **Reporting Output**: Flutter PDF & Printing Package APIs
* **Platform Integrations**: Android SDK, Share Plus, File Selector
* **Tooling**: Git & GitHub

---

## 🚀 Core Features

* **Customer Ledger Management**: Organize and view transaction statements of all active merchants in one centralized list.
* **Outstanding Balance Tracking**: Instantly calculates and displays cumulative outstanding receivables by customer.
* **Sales Recording**: Log credit sales with specific article numbers, colors, rates, and quantities.
* **Collection Tracking**: Track customer payments via Cash, Bank Transfer, UPI, or Cheque.
* **Invoice Generation**: Build itemized billing sheets instantly with automated net subtotal calculations.
* **PDF Export**: Generate professional vector PDF invoices and ledger statements.
* **Google Sign-In**: Secure user registration and session management.
* **Offline Database**: Offline relational data storage with foreign key constraints.
* **Backup & Restore**: Export local databases (`shoe_ledger_backup.db`) and restore them seamlessly.
* **Business Reporting**: Aggregated sales and collection logs filterable by date parameters.

---

## 🔄 Business Workflow

The flow of operational data in the app follows this sequence:

```
Authentication
      ↓
Customer Management
      ↓
Sales Recording
      ↓
Collections Recording
      ↓
Balance Tracking
      ↓
Invoice Generation
      ↓
PDF Reports
```

---

## 🏗️ Architecture Section

The software architecture is decoupled into distinct layers to ensure separation of concerns and high performance:

```
Flutter UI Layer (Material 3 Widgets)
      ↓
Business Logic Layer (Controllers & AuthService APIs)
      ↓
SQLite Database Layer (Local Sqflite persistence)
      ↓
PDF Generation Layer (Vector rendering and OS printing)
```

---

## 📄 PDF Reporting Workflow
The application generates high-fidelity, vector-based PDF invoices and ledger summaries programmatically using a custom canvas layout:

1. **Aggregation**: Gathers metadata (customer profiles, shop settings, transaction dates) and aggregates calculations (sums, net balances).
2. **Layout Compilation**: Arranges headers, item tables, and footers dynamically inside multi-page document containers.
3. **Android Channel Dispatch**: Leverages the system printing APIs to output PDF files or share them natively via WhatsApp/Email.

📂 **[Download Sample PDF Report Document](./docs/sample_party_ledger_report.pdf)**

---

## 📱 Application Gallery

### Launch & Authentication
| Splash Screen | Login Screen | Settings & Database Utilities |
| :---: | :---: | :---: |
| <img src="./screenshots/01_splash_screen.jpeg" width="220" alt="Splash Screen"/> | <img src="./screenshots/02_login_screen.jpeg" width="220" alt="Login Screen"/> | <img src="./screenshots/12_settings_backup_restore.jpeg" width="220" alt="Settings Screen"/> |
| Slate dark gradient with animated fade-in. | Backdrop filter blur with Google integration. | Reorganized sections for profile, backups, and about. |

### Dashboard Analytics
| Dashboard Overview | Metrics Cards | Recent Transactions Feed |
| :---: | :---: | :---: |
| <img src="./screenshots/03_dashboard_overview.jpeg" width="220" alt="Dashboard Overview"/> | <img src="./screenshots/04_dashboard_metrics.jpeg" width="220" alt="Dashboard Metrics"/> | <img src="./screenshots/05_recent_transactions.jpeg" width="220" alt="Recent Transactions"/> |
| At-a-glance receivables summary. | Spaced cards with custom elevations. | List of latest database transactions. |

### Ledgers & Entry Records
| Customer Ledger Directory | Credit Sale Entry | Payment Entry |
| :---: | :---: | :---: |
| <img src="./screenshots/06_party_ledger.jpeg" width="220" alt="Party Ledger"/> | <img src="./screenshots/11_Add_sale.jpeg" width="220" alt="Add Sale"/> | <img src="./screenshots/10_payment_entry.jpeg" width="220" alt="Payment Entry"/> |
| Sorted customer credit statements. | Log credit sales with article codes. | Track customer collections. |

### Invoices & Reports
| Invoice Generation Form | Invoice History Log | Daily Sales Log | Balance Receivables Overview |
| :---: | :---: | :---: | :---: |
| <img src="./screenshots/07_invoice_creation.jpeg" width="180" alt="Invoice Creation"/> | <img src="./screenshots/08_invoice_history.jpeg" width="180" alt="Invoice History"/> | <img src="./screenshots/09_daily_sales_report.jpeg" width="180" alt="Daily Sales Report"/> | <img src="./screenshots/13_balance_tracking.jpeg" width="180" alt="Balance Tracking"/> |
| Itemized billing input form. | List of historically built bills. | Filtered sales summaries. | Receivable logs by customer profile. |

---

## ⬇️ Download Android APK

The latest Android release APK is available for installation.

📥 **[Download Kritika Business Ledger v1.0 APK](./releases/Kritika-Business-Ledger-v1.0.apk)**

### APK Installation Instructions
1. Download the `Kritika-Business-Ledger-v1.0.apk` file on your Android device.
2. Locate the file in your device's File Manager and tap to install.
3. If prompted, enable "Install from Unknown Sources" in your browser/file manager settings.
4. Open the application and configure your first business profile.

---

## 💡 Development Highlights
* **High Linter Compliance**: Verified 100% warning-free under `flutter analyze` configurations.
* **Robust Widget Testing**: Features automated smoke-testing verification scripts (`flutter test`) verifying widget layout trees.
* **Error Mapping**: Decouples API client exceptions into user-friendly prompts for connectivity issues, authentication timeouts, and database access errors.
* **Asset Resilience**: Utilizes fallback UI builders that automatically render premium linear gradients and icons if physical logo files are missing.

---

## 🏆 Engineering Highlights
- Flutter-based cross-platform architecture.
- Firebase Authentication with Google Sign-In support.
- Offline-first SQLite persistence layer with relational integrity.
- Professional PDF invoice and ledger generation.
- Backup & Restore functionality for local database recovery.
- Mobile-first Material 3 UX design.
- Production-ready Android release build setups.
- Real-world manufacturing and distribution business use case mapping.

---

## 📈 Key Achievements
- Designed and developed a complete Flutter business application from concept to deployment.
- Implemented offline-first architecture using SQLite for reliable local data storage.
- Integrated Firebase Authentication and Google Sign-In for secure access.
- Built professional PDF invoice and ledger generation workflows.
- Developed backup and restore functionality for business continuity.
- Successfully generated production Android release builds (APK & AAB).
- Applied real-world business workflow modeling based on manufacturing and distribution operations.

---

## 🔮 Future Enhancements
* **Dark Mode Support**: Add a modern dark theme to improve readability under low-light conditions.
* **Inventory Module**: Track shoe model sizes, cartons, and stock counts.
* **Analytics Dashboard**: Add charts showing sales trends and monthly collections.
* **Cloud Synchronization**: Sync local data with a remote database (Firestore) with full offline caching.
* **Multi-user Support**: Role-based access controls for business owners and sales agents.

---

## 📊 Project Statistics
* **Platform**: Android
* **Framework**: Flutter
* **Language**: Dart
* **Authentication**: Firebase Authentication
* **Database**: SQLite
* **Reporting**: PDF Generation
* **Architecture**: Layered Mobile Application Architecture
* **Offline Support**: Yes
* **Release Build**: APK + AAB

---

## 🔒 Source Code Notice
The complete source code is maintained in a private repository. This public repository serves as a product showcase, documentation hub, screenshots gallery, and APK distribution page.
