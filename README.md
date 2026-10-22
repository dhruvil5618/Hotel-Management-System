🏨 Hotel Management System in C++

A simple, menu-driven Hotel Management System developed using C++. This project demonstrates the practical implementation of Object-Oriented Programming (OOP) concepts, including inheritance, polymorphism, encapsulation, and constructors.

The system allows users to manage hotel rooms, register customers, make room bookings, process checkouts, generate bills, and view the final hotel report.

📌 Project Overview

The Hotel Management System is designed to simplify basic hotel operations through a console-based application. It provides a structured way to manage room availability, customer information, booking details, and payment records.

The project is developed as an academic project to understand the application of C++ programming and OOP concepts in a real-world scenario.

✨ Features

- Room Management: Display available and occupied rooms with their types and prices.
- Customer Registration: Register customers with their name, phone number, and email address.
- Room Booking: Book an available room using a registered customer's ID.
- Customer Management: Display registered customer details.
- Checkout System: Process checkout by entering the checkout date and number of nights stayed.
- Bill Generation: Calculate the total room charges based on the room price and number of nights.
- Payment Options: Choose between Cash and UPI.
- Payment Confirmation: Confirm payment before completing checkout.
- Room Availability Updates: Automatically update room status after booking and checkout.
- Final Hotel Report: Display booking records, completed checkouts, and total revenue.
- Input Validation: Validate phone number format, basic email format, booking details, and payment selection.

🛏️ Room Details

The system contains four predefined rooms.

Room Number| Room Type| Price Per Night
101| Standard| ₹1,500
201| Deluxe| ₹2,500
301| Deluxe| ₹2,500
401| Premium Suite| ₹6,000

Note: Room prices are predefined in the program and can be modified in the corresponding room classes.

🛠️ Technologies Used

- Programming Language: C++
- Programming Concepts: Object-Oriented Programming
- Standard Libraries: "iostream", "string", "iomanip"
- Compiler: GCC or any compatible C++ compiler
- Development Environment: Any C++ IDE or code editor

🧠 OOP Concepts Implemented

This project demonstrates the following Object-Oriented Programming concepts.

1. Encapsulation

The "Customer" class stores customer information using private data members. Access to selected information is provided through public member functions.

2. Inheritance

The "StandardRoom", "DeluxeRoom", and "PremiumSuite" classes inherit from the base "Room" class.

This allows the derived classes to reuse the common room properties and functions.

3. Polymorphism

The "Room" class contains virtual functions such as "calculateBill()" and "display()".

The derived room classes override "calculateBill()". The program uses a base-class pointer to call the appropriate virtual function at runtime.

4. Constructors

Constructors initialize room details and customer information when objects are created.

5. Abstraction

The "Hotel" class organizes hotel operations into separate functions, such as "registerCustomer()", "bookRoom()", "checkOut()", and "finalReport()".

This separates the main operations from the menu interface.

📂 Project Structure

Hotel-Management-System/
│
├── main.cpp
└── README.md

Note: Replace "main.cpp" with your actual C++ source filename if it is different.

⚙️ How to Run the Project

Step 1: Clone the Repository

Open your terminal and execute:

git clone YOUR_GITHUB_REPOSITORY_URL

Replace "YOUR_GITHUB_REPOSITORY_URL" with your actual GitHub repository URL.

Step 2: Open the Project Folder

cd Hotel-Management-System

Step 3: Compile the Program

If you have GCC installed, run:

g++ -std=c++11 main.cpp -o hotel

Step 4: Run the Program

On Windows:

hotel.exe

On Linux or macOS:

./hotel

You can also compile and run the code using an IDE or an online C++ compiler that supports C++11.

🚀 How to Use the System

After running the program, the following menu appears:

===== HOTEL MANAGEMENT SYSTEM =====
1. Display Rooms
2. Register Customer
3. Book Room
4. Check Out and Generate Bill
5. Display Customers
0. Exit and Generate Final Report
Enter Choice:

Step-by-Step Workflow

1. Display Rooms: View room numbers, types, prices, and availability.
2. Register Customer: Enter the customer's name, 10-digit phone number, and email address.
3. Book Room: Enter the registered customer ID, select an available room, and provide the check-in date.
4. Check Out: Enter the room number, checkout date, and number of nights stayed.
5. Select Payment: Choose Cash or UPI and confirm the payment.
6. Generate Bill: View the total amount, booking details, payment method, and checkout confirmation.
7. View Customers: Display all registered customers.
8. Generate Final Report: Select option "0" to display booking records, completed checkouts, and total revenue before exiting.

💰 Billing Calculation

The total room charge is calculated using the following formula:

Total Bill = Room Price Per Night × Number of Nights Stayed

Example

Suppose a customer books a Deluxe room for 3 nights.

- Room Type: Deluxe
- Price Per Night: ₹2,500
- Number of Nights: 3

Calculation:

Total Bill = 2500 × 3
           = ₹7,500

The program calculates the bill using the "calculateBill()" function defined in the room classes.

📊 Final Hotel Report

When the user exits the application, the system generates a final report containing:

- Customer IDs associated with bookings
- Room numbers
- Check-in and checkout dates
- Number of nights for completed bookings
- Payment methods
- Booking status
- Total revenue from completed checkouts

Bookings that have not completed checkout are displayed as currently occupied.

⚠️ Current Limitations

This project is a basic console-based hotel management application. Its current limitations include:

- Customer and booking records are stored in memory and are not saved permanently.
- Room booking dates are entered manually.
- The program does not automatically calculate the number of nights from the check-in and checkout dates.
- The system supports only four predefined rooms.
- Phone and email validation checks basic formatting rather than verifying actual contact details.
- The program does not integrate with a real payment gateway.
- The application does not support simultaneous users or online reservations.

These limitations can be addressed in future versions.

🔮 Future Improvements

Possible improvements include:

- Database integration for permanent storage.
- Automatic calculation of nights from dates.
- Dynamic room and customer management.
- Improved input validation.
- Booking cancellation and modification.
- A graphical user interface (GUI).
- Online room reservation functionality.
- Integration with a payment gateway.

🎯 Project Objective

The primary objective of this project is to apply C++ programming fundamentals and Object-Oriented Programming concepts to develop a practical hotel management application.

It also helps demonstrate how classes, inheritance, polymorphism, and data organization can be used to manage real-world operations.

👨‍💻 Author

Developed as an academic C++ project.

GitHub Repository: YOUR_GITHUB_REPOSITORY_URL

---

⭐ If you find this project useful for learning C++ and Object-Oriented Programming, consider giving the repository a star!
