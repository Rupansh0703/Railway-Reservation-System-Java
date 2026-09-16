# 🚆 Terminal-Based Rail Reservation System

## 📝 Project Description
The Rail Reservation System is a terminal-based application developed using Core Java. It provides basic railway reservation facilities for users and administrators.

The project does not use an external database. All data is stored persistently using Java File Handling and text files.

## 🎯 Objectives
- Develop a railway reservation system using Core Java.
- Implement Object-Oriented Programming concepts.
- Provide separate User and Admin functionalities.
- Implement train searching and ticket booking.
- Automatically generate PNR and seat numbers.
- Store application data using text files.
- Implement custom exception handling.

## ✨ User Features
- User Registration
- User Login
- Search Trains
- View All Trains
- Check Seat Availability
- Book Tickets
- Automatic PNR Generation
- Automatic Seat Assignment
- View Ticket using PNR
- View Booking History
- Cancel Ticket

## 👑 Admin Features
- Admin Login
- Add Train
- Update Train
- Delete Train
- View All Trains
- View All Bookings

## 🧠 Java Concepts Used
- Classes and Objects
- Encapsulation
- Inheritance
- Abstraction
- Polymorphism
- Interfaces
- Method Overriding
- Comparable
- ArrayList
- Collections
- File Handling
- Exception Handling
- Custom Exceptions
- User-Defined Packages

## 🔄 Train Management
The administrator can add, update, and delete trains. Each train contains:
- Train Number
- Train Name
- Source
- Destination
- Total Seats
- Fare

The `Train` class implements `Comparable<Train>` and trains are sorted according to their train number.

## 🎫 Ticket Booking
During ticket booking, the system stores:
- PNR
- User ID
- Train Number
- Passenger ID
- Seat Number
- Fare
- Status

The system automatically generates a unique PNR and assigns an available seat.

## 💺 Seat Management
The system checks confirmed bookings before assigning a seat. If no seat is available, `SeatNotAvailableException` is generated.

When a ticket is cancelled, its seat becomes available again.

## ⚠️ Custom Exceptions
The project contains the following custom exceptions:
- `TrainNotFoundException`
- `SeatNotAvailableException`
- `TicketNotFoundException`

These exceptions are used to handle application-specific errors.

## 💾 File Handling
The project uses Java File Handling instead of an external database.

Classes used:
- `File`
- `FileReader`
- `FileWriter`
- `BufferedReader`
- `BufferedWriter`

The `data` folder stores all application records.

## 📂 Project Structure

RailReservationSystem/
│
├── src/
│   ├── Main.java
│   ├── model/
│   │   ├── Person.java
│   │   ├── Train.java
│   │   ├── Passenger.java
│   │   ├── Ticket.java
│   │   └── User.java
│   │
│   ├── service/
│   │   ├── ReservationSystem.java
│   │   ├── TrainService.java
│   │   ├── TicketService.java
│   │   └── UserService.java
│   │
│   ├── exception/
│   │   ├── SeatNotAvailableException.java
│   │   ├── TrainNotFoundException.java
│   │   └── TicketNotFoundException.java
│   │
│   └── util/
│       ├── FileManager.java
│       ├── InputHelper.java
│       └── PNRGenerator.java
│
├── data/
│   ├── users.txt
│   ├── trains.txt
│   ├── tickets.txt
│   └── passengers.txt
│
└── README.md

## 📦 Package Description

### model
Contains the main entity classes such as `Train`, `User`, `Passenger`, `Ticket`, and `Person`.

### service
Contains the main business logic for users, trains, tickets, and the reservation system.

### exception
Contains custom exception classes used for handling errors.

### util
Contains utility classes for file handling, input handling, and PNR generation.

## 💻 Technologies Used

| Technology | Purpose |
|---|---|
| Core Java | Application Development |
| OOP | Program Structure |
| ArrayList | Data Management |
| Comparable | Train Sorting |
| File Handling | Data Storage |
| Exception Handling | Error Handling |
| Terminal | User Interface |

## 🚀 How to Run

Open the terminal inside the `src` folder.

Compile the complete project:

javac Main.java model\*.java service\*.java exception\*.java util\*.java

Run the application:

java Main

## 🔐 Default Admin

User ID: `A001`  
Username: `admin`  
Password: `admin123`  
Role: `ADMIN`

## 📊 Data Storage

`users.txt` stores user and admin information.

`trains.txt` stores train information.

`tickets.txt` stores ticket and booking information.

`passengers.txt` stores passenger information.

## 🔮 Future Enhancements
- MySQL database integration
- Graphical User Interface
- Web-based application
- Password encryption
- Online payment
- Train schedules
- Different classes of seats
- Email/SMS notifications
- Multiple passengers per booking

## 📌 Conclusion

The Rail Reservation System demonstrates the practical implementation of Core Java concepts in a real-world application. It combines OOP, Collections, File Handling, Exception Handling, Comparable, and User-Defined Packages to provide a simple railway reservation system.

The project is designed for easy understanding, college submission, demonstration, and viva preparation.

## 👨‍💻 Author

**Rupansh Patidar**  
**Registration No.: 25BAI11498**