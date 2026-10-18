# 💰 Personal Expense Tracker

<p align="center">
  <b>Take control of your finances with a smart, offline expense tracking app.</b>
</p>

<p align="center">
  <em>"A modern Android application built in Java to track daily expenses, view transaction history, and analyze spending habits using SQLite."</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Made%20with-%E2%9D%A4%EF%B8%8F-red" alt="Made with Love">
  <img src="https://img.shields.io/badge/Platform-Android-green" alt="Platform">
  <img src="https://img.shields.io/badge/Language-Java-orange" alt="Language">
  <img src="https://img.shields.io/badge/Database-SQLite-blue" alt="Database">
  <img src="https://img.shields.io/badge/Status-Complete-success" alt="Status">
</p>

---

## 📋 Overview

**Personal Expense Tracker** is a feature-rich, offline Android application designed to help users manage their daily finances. Built entirely in **Java**, it allows users to log incomes and expenses, categorizes them, and provides a clear visual breakdown of where the money is going. All data is stored locally using **SQLite**, ensuring complete privacy and offline access.

---

## ✨ Key Features

* **💸 Add Transactions:** Easily log income and expenses with details like amount, category, date, and notes.
* **📊 Analytics & Insights:** Visual representation (charts/graphs) of spending habits across different categories.
* **📜 History:** View a complete, scrollable list of all past transactions using a custom `RecyclerView` adapter.
* **📱 Bottom Navigation:** Seamlessly switch between Home, History, and Analytics using a modern bottom navigation bar.
* **🗄️ Local Database:** Uses `SQLiteOpenHelper` for robust, offline data storage. No internet required!
* **🎨 Clean UI:** Modern UI with custom drawables, colors, and dark mode support (`values-night`).

---

## 🛠️ Tech Stack

| Category | Tools / Technologies |
|---|---|
| **Language** | Java |
| **IDE** | Android Studio |
| **Database** | SQLite (`SQLiteOpenHelper`) |
| **UI Components** | Fragments, RecyclerView, BottomNavigationView |
| **Architecture** | Model-View-Adapter (MVA) |
| **Design** | XML Layouts, Custom Drawables, Material Design |

---

## 📂 Project Structure

```text
android-personal-expense-tracker/
│
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/expense/tracker/
│   │   │   │   ├── adapter/
│   │   │   │   │   └── TransactionAdapter.java  # RecyclerView Adapter
│   │   │   │   ├── database/
│   │   │   │   │   └── DatabaseHelper.java      # SQLite Database Management
│   │   │   │   ├── model/
│   │   │   │   │   └── Transaction.java         # Data Model
│   │   │   │   ├── AddTransactionActivity.java  # Add Income/Expense
│   │   │   │   ├── AnalyticsFragment.java       # Spending Analytics
│   │   │   │   ├── HistoryFragment.java         # Transaction History
│   │   │   │   ├── HomeFragment.java            # Dashboard
│   │   │   │   └── MainActivity.java            # Main Host Activity
│   │   │   ├── res/
│   │   │   │   ├── color/                       # Color state lists
│   │   │   │   ├── drawable/                    # Icons & custom shapes
│   │   │   │   ├── layout/                      # UI Layouts (activity, fragment, item)
│   │   │   │   ├── menu/                        # Bottom nav menu
│   │   │   │   ├── mipmap-anydpi-v26/           # Adaptive launcher icons
│   │   │   │   ├── values/                      # Colors, Strings, Themes
│   │   │   │   └── values-v23/                  # Theme overrides for API 23+
│   │   │   └── AndroidManifest.xml
│   │   └── build.gradle
│   ├── proguard-rules.pro
│   └── gradle/
├── build.gradle
├── settings.gradle
└── README.md
```

---

## 🚀 How to Build and Run

### Prerequisites
* **Android Studio** (Latest Version)
* **JDK 11** or higher
* **Android SDK** (API 24+)

### Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/iqramaaqsoodmughal363/android-personal-expense-tracker.git
   ```
2. **Open in Android Studio**
   Open Android Studio → **File** → **Open** → Select the project folder.
3. **Sync Gradle**
   Wait for Gradle to sync. Click **"Sync Now"** if prompted.
4. **Build and Run**
   Connect your Android device or start an emulator, then click the **Run** button (green play icon).

---

## ⚙️ How It Works (Behind the Scenes)

### 1. Data Persistence (`DatabaseHelper.java`)
The app uses SQLite to store all transactions. It creates a table with columns for ID, Amount, Category, Date, Type (Income/Expense), and Notes. It provides CRUD (Create, Read, Update, Delete) methods to manage data efficiently.

### 2. Dynamic Lists (`TransactionAdapter.java`)
The `HistoryFragment` uses a `RecyclerView` to display the transaction list. The `TransactionAdapter` binds the SQLite data to the custom item layout, ensuring smooth scrolling even with hundreds of records.

### 3. Modular UI (`MainActivity.java` & Fragments)
The `MainActivity` hosts a `BottomNavigationView` and a `FragmentContainerView`. Based on the user's selection, it replaces the fragments (`Home`, `History`, `Analytics`) without restarting the activity.

---

## 🎯 Key Takeaways

* **Offline First:** Complete privacy, as no data is sent to any external server.
* **Clean Architecture:** Separation of concerns using Models, Database Helpers, and Adapters.
* **Practical Java:** Demonstrates core Java skills (OOP, Collections, Exception Handling) in an Android context.
* **Modern UI:** Utilizes Material Design components like Bottom Navigation and Cards.

---

## 👩‍💻 Author

**Iqra Maqsood Mughal**

*Software Engineer · Full-Stack Developer · Code Craftsman · Android App Developer · Problem Solver 🚀*

```javascript
const codeIsLife = "Code is life";
while (true) { 
    learn(); 
    build(); 
    innovate(); 
}
```

---

## 📅 Date

October 18, 2026

---

## 📄 License

This project is intended for educational and personal use purposes.
```
