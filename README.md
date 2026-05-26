# **Flutter News App**

A **Flutter mobile news application** that fetches articles from an external news API and allows users to read, view details, and save favorite articles locally.

The app is built with **Flutter**, uses the **HTTP package** to consume a news API, and stores favorite articles locally using **SQFlite**.

---

# **Project Purpose**

The purpose of this project is to build a simple and functional mobile news application using Flutter.

The application allows users to:

- **View daily news**
- **Read article titles and descriptions**
- **Open article details**
- **See article images**
- **View author and publication date**
- **Add articles to favorites**
- **Remove articles from favorites**
- **Store favorites locally on the device**

This project can be used as a foundation for:

- **Flutter news applications**
- **Mobile API consumption projects**
- **Offline favorites apps**
- **SQLite / SQFlite learning projects**
- **News reader apps**
- **Student Flutter projects**
- **Portfolio mobile applications**

---

# **Technologies Used**

## **Mobile Framework**

- **Flutter**
- **Dart**

## **API & Data**

- **HTTP**
- **NewsAPI**
- **JSON decoding**

## **Local Storage**

- **SQFlite**
- **SQLite**
- **Shared Preferences**

## **UI & Utilities**

- **Material Design**
- **Intl**
- **Carousel Slider**

---

# **Main Features**

## **Splash Screen**

The app starts with a splash screen before navigating to the home page.

---

## **News List**

The home screen displays a list of news articles fetched from an external API.

Each article card shows:

- **Title**
- **Short description**
- **Favorite icon**
- **Card-based layout**

---

## **Article Details**

Users can open an article to view more information:

- **Article title**
- **Article image**
- **Author**
- **Publication date**
- **Description**
- **Favorite button**

---

## **Favorites System**

The app allows users to save articles locally.

Users can:

- **Add an article to favorites**
- **Remove an article from favorites**
- **Check if an article is already saved**
- **Open the favorites page**
- **Persist favorites even after closing the app**

---

## **Local Database**

The app uses a local SQLite database through SQFlite.

Stored article fields:

- **title**
- **description**
- **imageUrl**
- **publishedAt**
- **author**

---

# **Project Structure**

```bash
flutterapi/
├── android/
├── ios/
├── lib/
│   ├── database/
│   │   └── database_helper.dart
│   │
│   ├── screens/
│   │   ├── splash_screen.dart
│   │   ├── home_screen.dart
│   │   ├── article_detail_screen.dart
│   │   └── favorites_screen.dart
│   │
│   └── main.dart
│
├── assets/
│   ├── splash.png
│   ├── logo.png
│   ├── image1.png
│   ├── image2.png
│   └── image3.png
│
├── pubspec.yaml
└── README.md
```

---

# **Application Flow**

## **1. App Start**

The app starts from:

```dart
main.dart
```

It launches:

```dart
SplashScreen()
```

---

## **2. Home Screen**

After the splash screen, the user reaches the home screen.

The home screen fetches articles from the news API and displays them in a list.

---

## **3. Article Selection**

When the user taps an article, the app opens the article details page.

---

## **4. Add to Favorites**

The user can add the article to local favorites.

The article is stored in the local SQLite database.

---

## **5. Favorites Page**

The user can open the favorites page and see saved articles.

---

# **API Used**

The application uses **NewsAPI** to fetch articles.

Example API source used in the project:

```text
https://newsapi.org/v2/everything?domains=wsj.com
```

---

# **Local Database**

The local database is named:

```text
news.db
```

The favorites table is named:

```text
favorites
```

Table fields:

```text
id
title
description
imageUrl
publishedAt
author
```

---

# **Installation**

## **1. Clone the Repository**

```bash
git clone https://github.com/Noris69/flutterapi.git
cd flutterapi
```

---

## **2. Install Dependencies**

```bash
flutter pub get
```

---

## **3. Run the Application**

```bash
flutter run
```

---

# **Useful Commands**

## **Install dependencies**

```bash
flutter pub get
```

## **Run app**

```bash
flutter run
```

## **Analyze code**

```bash
flutter analyze
```

## **Run tests**

```bash
flutter test
```

## **Build Android APK**

```bash
flutter build apk
```

## **Build iOS**

```bash
flutter build ios
```

---

# **Assets**

The project includes the following assets:

```text
assets/splash.png
assets/logo.png
assets/image1.png
assets/image2.png
assets/image3.png
```

These assets are declared in `pubspec.yaml`.

---

# **Security Recommendations**

- **Do not hardcode API keys directly in source code**
- **Move the NewsAPI key to a secure configuration file**
- **Use environment variables or build-time configuration**
- **Do not commit sensitive keys to GitHub**
- **Regenerate the exposed API key if needed**
- **Handle API errors gracefully**
- **Add loading and empty states**

---

# **Git Ignore Recommendations**

```gitignore
.dart_tool/
build/
.packages
.pub-cache/
.pub/
.flutter-plugins
.flutter-plugins-dependencies
.idea/
.vscode/
*.log
.env
```
---

# **Author**

Developed by **Noris69**.
