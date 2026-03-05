# 🚖 Call Taxi Booking Application

## 📌 Project Description

The **Call Taxi Booking Application** is a Java-based console application that simulates a taxi booking system operating on a linear route. Customers can book taxis between predefined points, and the system automatically allocates the most suitable taxi based on availability, location, and earnings.

This project demonstrates **object-oriented programming concepts, service-layer architecture, and basic scheduling logic**.

---

## 🧾 Problem Assumptions

* Number of taxis: **4**
* Route points: **A, B, C, D, E, F**
* Distance between each point: **15 km**
* Travel time between points: **60 minutes**
* Initial taxi location: **All taxis start at point A**

### 💰 Fare Calculation

* Minimum charge: **₹100 for first 5 km**
* Additional charge: **₹10 per km after 5 km**

---

## ⚙️ Booking Rules

1. If a taxi is **available at the pickup point**, it is allocated.
2. If no taxi is available at the pickup point, the **nearest free taxi** is allocated.
3. If multiple taxis are available at the same location, the **taxi with lower total earnings** is selected.
4. Fare is calculated **only between pickup and drop points**.
5. If no taxi is available, **booking is rejected**.

---

## 🏗️ Project Structure

```
Call Taxi Booking Application
│
├── src
│   ├── com.calltaxi.main
│   │   └── Main.java
│   │
│   ├── com.calltaxi.model
│   │   ├── Booking.java
│   │   └── Taxi.java
│   │
│   └── com.calltaxi.service
│       └── TaxiService.java
```

---

## 📦 Package Explanation

### `com.calltaxi.main`

Contains the **Main class** which runs the application and handles user interaction.

**File**

* `Main.java` → Entry point of the program.

---

### `com.calltaxi.model`

Contains **data model classes** used in the application.

**Files**

* `Taxi.java` → Represents taxi details such as

  * Taxi ID
  * Current location
  * Total earnings
  * Booking history

* `Booking.java` → Represents booking information such as

  * Booking ID
  * Customer ID
  * Pickup point
  * Drop point
  * Pickup time
  * Drop time
  * Fare amount

---

### `com.calltaxi.service`

Contains the **business logic of the application**.

**File**

* `TaxiService.java`

  * Taxi allocation logic
  * Fare calculation
  * Booking creation
  * Display taxi details

---

## 🧠 Features

* Automatic taxi allocation
* Nearest taxi selection
* Taxi earnings tracking
* Booking history maintenance
* Fare calculation based on distance
* Display taxi booking details

---

## 🖥️ Sample Booking

```
Customer ID: 1
Pickup: A
Drop: B
Pickup Time: 9
```

Output:

```
Taxi can be allotted.
Taxi-1 is allotted.
```

---

## 📊 Taxi Details Output Example

```
Taxi-1  Total Earnings: Rs.400

BookingID   CustomerID   From   To   PickupTime   DropTime   Amount
1           1            A      B    9            10         200
3           3            B      C    12           13         200
```

---

## 🛠️ Technologies Used

* Java
* Object-Oriented Programming
* Console-based application

---

## ▶️ How to Run the Project

1. Clone the repository
2. Import the project into **Eclipse / IntelliJ IDEA**
3. Navigate to:

```
com.calltaxi.main.Main
```

4. Run the **Main.java** file

---

## 🎯 Learning Outcome

This project helps in understanding:

* Java class design
* Package structuring
* Service layer implementation
* Real-time allocation logic
* Object-oriented programming principles

---

output:

<img width="1016" height="841" alt="Screenshot 2026-03-05 091944" src="https://github.com/user-attachments/assets/579337cb-9268-4667-a120-4f7a64af759e" />


## 👨‍💻 Author

Student Project – Call Taxi Booking Application
