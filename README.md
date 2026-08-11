# 🚗 Crews Auto - On-Demand Roadside & Automotive Service Platform

[![Flutter](https://img.shields.io/badge/Flutter-3.0+-02569B?style=for-the-badge&logo=flutter&logoColor=white)](https://flutter.dev)
[![Dart](https://img.shields.io/badge/Dart-3.0+-0175C2?style=for-the-badge&logo=dart&logoColor=white)](https://dart.dev)
[![Firebase](https://img.shields.io/badge/Backend-Firebase_Firestore-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)](https://firebase.google.com)
[![State Management](https://img.shields.io/badge/State_Management-Provider-blue?style=for-the-badge)](https://pub.dev/packages/provider)
[![License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](LICENSE)

A full-stack, cross-platform **Flutter & Firebase Automotive Service Ecosystem** connecting vehicle owners with professional mechanics and workshop administrators in real-time for roadside emergency assistance, periodic maintenance, and repairs.

---

## 🌟 Multi-Role System Architecture

                            ┌───────────────────────────────┐
                            │     🛡️ Admin Control Portal   │
                            │  - Dispatch & Request Manager │
                            │  - Mechanic Verification      │
                            │  - Category & Pricing Config  │
                            └───────────────┬───────────────┘
                                            │
             ┌──────────────────────────────┴──────────────────────────────┐
             │                                                             │
             ▼                                                             ▼
┌─────────────────────────────────┐ ┌─────────────────────────────────┐ │ 🚗 User / Vehicle Owner │ Firebase Cloud Sync │ 🔧 Mechanic / Technician │ │ - Book Breakdown Assistance │ ◄───────────────────────► │ - Real-Time Breakdown Alerts │ │ - AI Diagnostic Chatbot │ (Firestore / Storage) │ - GPS Route & Task Details │ │ - Digital Tickets & Payments │ │ - Live Job Execution & Finish │ └─────────────────────────────────┘ └─────────────────────────────────┘



---

## ✨ Key Features

### 🚗 1. Vehicle Owner (Customer) Module
* **🚨 Emergency Roadside Assistance:** Quick-request assistance for tire punctures, engine overheating, battery jumpstarts, and towing.
* **🛠️ Scheduled Maintenance:** Book complete car service packages, oil replacement, brake checks, and sound system installations.
* **🤖 Integrated AI Automotive Chatbot:** Immediate interactive assistance to troubleshoot car warning lights and mechanical issues.
* **🎫 Digital Service Tickets:** Real-time visibility into repair progress, assigned technician info, and completion status.
* **💳 Secure Payments & Invoicing:** Add credit/debit cards and checkout securely with instant invoice generation.
* **⭐ Star Ratings & Reviews:** Rate mechanic performance and leave detailed service feedback.

### 🔧 2. Mechanic / Technician Module
* **📲 Real-Time Job Dispatch:** Receive instant breakdown assignment notifications with customer location and fault details.
* **📍 Live Work Mode (`live.dart`):** Start jobs, record parts replaced, and update live repair status for the customer.
* **📊 Job History & Completed Tasks:** Monitor completed jobs, customer ratings, and daily earnings.
* **👤 Technician Profile:** Manage personal information, specialization, and availability status.

### 🛡️ 3. Administrator Portal
* **📈 Operations Dashboard:** Live analytics tracking active requests, completed tickets, active mechanics, and platform metrics.
* **👨‍🔧 Mechanic Management:** Add, verify, and monitor mechanic credentials (`AddMechanicScreen.dart`, `TotalMechanics.dart`).
* **📦 Service Category Management:** Add and update service categories, descriptions, and standard repair costs.

---

## 📂 Project Structure
lib/ ├── main.dart # App bootstrap & Firebase initialization ├── firebase_options.dart # Multi-platform Firebase configuration ├── Authentication/ # Role-based login & signup (User/Mechanic/Admin) │ ├── User/ # Vehicle owner experience │ ├── data/pages/ # Screens (home, service form, ticket, chatbot, payments) │ ├── component/ # Bottom navigation & user widgets │ └── Widgets/ # Custom scaffold & layout containers │ ├── Mechanic/ # Technician dashboard & job workflows │ ├── pages/ # Assigned tasks, live work view, completed jobs │ └── component/ # Mechanic cards & action buttons │ ├── Admin/ # Admin control center │ ├── Pages/ # Analytics dashboard, total requests, mechanic management │ ├── Model/ # Admin data models │ └── Provider/ # Admin state management │ ├── Provider/ # Application-wide state providers ├── models/ # Shared data entities (Service, User, Ticket) ├── constants/ # Design tokens, API endpoints & asset paths └── style/ # App themes, custom typography & color palettes

---

## 🛠️ Tech Stack & Dependencies

* **Frontend Framework:** [Flutter](https://flutter.dev) (Dart SDK `>=2.18.6 <4.0.0`)
* **State Management:** [`provider`](https://pub.dev/packages/provider)
* **Backend & Cloud:**
  * [`firebase_core`](https://pub.dev/packages/firebase_core) - Firebase configuration
  * [`firebase_auth`](https://pub.dev/packages/firebase_auth) - Role-based authentication
  * [`cloud_firestore`](https://pub.dev/packages/cloud_firestore) - Real-time database sync
  * [`firebase_storage`](https://pub.dev/packages/firebase_storage) - Vehicle damage photo uploads
* **UI & Utilities:**
  * [`google_fonts`](https://pub.dev/packages/google_fonts) - Modern typography
  * [`flutter_rating_bar`](https://pub.dev/packages/flutter_rating_bar) - Star ratings
  * [`cached_network_image`](https://pub.dev/packages/cached_network_image) - Image caching
  * [`table_calendar`](https://pub.dev/packages/table_calendar) - Appointment date picker

---

## 🚀 Getting Started

### 1. Prerequisites
* [Flutter SDK](https://docs.flutter.dev/get-started/install)
* Android Studio / VS Code
* A configured [Firebase Project](https://console.firebase.google.com/) with Firestore & Authentication enabled

### 2. Clone the Repository
```bash
git clone https://github.com/Yyshnav/Crews-Auto-.git
cd Crews-Auto-


---

### Steps to update on GitHub:
1. Open [Crews-Auto- on GitHub](https://github.com/Yyshnav/Crews-Auto-).
2. Click the **Pencil (Edit)** icon on `README.md`.
3. Paste the markdown content above and click **"Commit changes..."**.


