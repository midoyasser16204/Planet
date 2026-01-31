# 🌍 Planet

**Planet** is a Flutter mobile application developed as a **teamwork project**, designed to provide a scalable and maintainable trip management system with a smooth and modern user experience.

The application follows **Clean Architecture**, a **feature-first structure**, and integrates mapping, authentication, caching, and backend services to simulate a real-world production-ready system.

---

## 📌 Project Description

Planet allows users to authenticate, browse available trips, view trip details, manage bookings, track trip history, and update personal profiles.

Trip locations and routes are visualized using **OpenStreetMap**, enhancing the user experience with interactive maps.

The backend is built with **Laravel (PHP)** and exposes RESTful APIs for authentication, trip management, and user-related operations.

To improve performance and reduce unnecessary API calls, the app implements a **local caching layer** using **Hive**.

The project emphasizes:

* Clean code
* Separation of concerns
* Scalability
* Team collaboration

---

## 👥 Team Members

This project was developed collaboratively by:

* **Marwan Atef** – Flutter Developer
  GitHub: [https://github.com/Marwan9Atef](https://github.com/Marwan9Atef)

* **Mohamed Yasser** – Flutter Developer
  GitHub: [https://github.com/midoyasser16204e](https://github.com/midoyasser16204e)

* **Abdalla Ahmed** – Flutter Developer
  GitHub: [https://github.com/Abdalla-Ahmed-Aly](https://github.com/Abdalla-Ahmed-Aly)

* **Mohamed Nasser** – Backend Developer
  GitHub: [https://github.com/MohamedNasser00](https://github.com/MohamedNasser00)

---

## ✨ Features Overview

* 🔐 Authentication (Phone & Google)
* 🧳 Trip Management
* 📍 Trip Location & Maps
* 🚗 Trip Details & Extra Trips
* ❌ Trip Cancellation
* 👤 User Profile Management
* 🕒 Trip History
* 💾 Local Caching & Offline Optimization

---

## 📸 Screenshots

### Splash screen

<table>
<tr>
<td align="center"><b>First Splash</b><br><br><img src="images/first splash.png" width="250"/></td>
<td align="center"><b>Second Splash</b><br><br><img src="images/second splash.png" width="250"/></td>

</tr>
</table>

---

###  Authentication

<table>
<tr>
<td align="center"><b>Login</b><br><br><img src="images/login.png" width="250"/></td>
<td align="center"><b>Register</b><br><br><img src="images/register.png" width="250"/></td>
<td align="center"><b>Send Code</b><br><br><img src="images/send code.png" width="250"/></td>
<td align="center"><b>Verify Code</b><br><br><img src="images/verify code.png" width="250"/></td>
<td align="center"><b>Reset Password</b><br><br><img src="images/reset password.png" width="250"/></td>
  
</tr>
</table>

---

<table>
<tr>

<td align="center"><b>Get Location</b><br><br><img src="images/get location.png" width="250"/></td>
</tr>
</table>

---

###  Trip Features

<table>
<tr>
<td align="center"><b>Trips</b><br><br><img src="images/trips.png" width="250"/></td>
<td align="center"><b>Extra Trip</b><br><br><img src="images/extra trip.png" width="250"/></td>
<td align="center"><b>Pending Trip</b><br><br><img src="images/pending trip.png" width="250"/></td>
<td align="center"><b>Cancel Trip</b><br><br><img src="images/cancel trip.png" width="250"/></td>
</tr>
</table>



---

###  Profile

<table>
<tr>
<td align="center"><b>Profile</b><br><br><img src="images/profile.png" width="250"/></td>
<td align="center"><b>Edit Profile</b><br><br><img src="images/edit profile.png" width="250"/></td>
</tr>
</table>

---

## 🔐 Authentication Features

* Phone number & password login
* Google Sign-In
* OTP-based password reset
* Secure input validation
* Persistent login using cached data

---

## 🧳 Trip Features

* View available trips
* Trip details with seat selection
* Add extra trips
* Cancel booked trips
* View trip history
* Map-based trip visualization using OpenStreetMap

---

## 👤 Profile Features

* View user information
* Update profile details
* Display user-related trip data
* Cached profile data for fast loading

---

## 🛠️ Tech Stack

### 📱 Frontend (Mobile)

* Flutter (Dart)
* State Management: Bloc / Cubit
* Networking: Dio
* Dependency Injection: get_it / injectable
* Architecture: Clean Architecture
* Maps: OpenStreetMap (OSM)

---

### 💾 Caching & Local Storage

* Hive – Lightweight local database
* Custom Cache Layer:

  * Cache user data
  * Cache trip data
  * Clear cache on logout
  * Improve performance & reduce API calls

---

### 🖥 Backend

* PHP
* Laravel Framework
* RESTful APIs
* Authentication & Authorization

---

## 🧱 Architecture Overview

The project follows a **Feature-Based Clean Architecture** approach.

Each feature is isolated and divided into **Data**, **Domain**, and **Presentation** layers.

---

### 📁 Feature Structure

```
feature_name/
├── data/
│   ├── datasources/
│   ├── models/
│   ├── mappers/
│   └── repositories/
├── domain/
│   ├── entities/
│   ├── repositories/
│   └── usecases/
└── presentation/
    ├── cubit/
    ├── screens/
    └── widgets/
```

---

### 🔁 Layer Responsibilities

**Data Layer**

* Handles API requests and caching
* Maps raw data into domain entities
* Implements repository contracts

**Domain Layer**

* Pure business logic
* Independent from Flutter & external libraries

**Presentation Layer**

* UI & user interaction
* State management using Cubit

---

## 📂 Core Module

```
core/
├── cache/
├── di/
├── constants/
├── services/
├── utils/
├── theme/
└── widgets/
```

---

## 📂 Main Project Structure

```
lib/
├── core/
├── features/
│   ├── auth/
│   ├── trip/
│   ├── trip-detail/
│   ├── extra-trip/
│   ├── cancel-trip/
│   ├── history/
│   ├── profile/
│   └── location/
└── main.dart
```

---

## 🚧 Future Enhancements

* 📍 Real-time trip tracking
* 💳 Online payment integration
* 🔔 Push notifications
* 🌍 Multi-language support

---

## ⭐ Acknowledgment

Thanks to all team members for their collaboration and effort in building this project.

Special thanks to **Youssef Salah** for his support
GitHub: [https://github.com/YousefSalah1](https://github.com/YousefSalah1)

If you find this project useful, please consider giving it a **star ⭐**.





