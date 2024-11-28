# BusTicketManagementSystem

## Description
**BusTicketManagementSystem** is a Java-based application for managing bus ticket bookings. It provides essential functionalities such as booking tickets, retrieving ticket details, and canceling tickets. The project also implements custom exceptions for better error handling, ensuring a seamless user experience. 

This project demonstrates key Java programming concepts, including:
- Object-Oriented Programming (OOP)
- Exception handling
- Interfaces and abstraction
- Collections framework (e.g., HashMap for storing tickets)

## Features
- **Book a Ticket**: Reserve a ticket for a passenger on a specific bus.
- **Retrieve Ticket**: View details of an already booked ticket.
- **Cancel Ticket**: Remove a ticket from the booking system.
- **Custom Exceptions**: Handles scenarios like duplicate tickets, missing tickets, and invalid buses.
- **Unique Ticket Number Generator**: Ensures each ticket has a unique identifier.

## Project Structure
The project is organized into the following folders:

### **1. Exceptions**
Custom exceptions for handling error scenarios:
- `InvalidBusException.java`: Thrown when the specified bus is invalid or not found.
- `TicketAlreadyExistException.java`: Thrown when a ticket with the same number already exists.
- `TicketDoesNotPresentException.java`: Thrown when attempting to retrieve or cancel a non-existent ticket.

### **2. Service**
Core business logic and domain classes:
- `Bus.java`: Represents a bus with attributes like bus number, route, and capacity.
- `BusTicketManagement.java`: Implements the logic for booking, retrieving, and canceling tickets.
- `Passenger.java`: Represents a passenger with attributes like name and age.
- `SeniorCitizen.java`: Extends `Passenger` to include a discount attribute.
- `Ticket.java`: Represents a bus ticket with details like ticket number, passenger, and bus.

### **3. Test**
Testing functionality:
- `Testing.java`: Contains a `main` method to test the booking, retrieval, and cancellation of tickets.

### **4. Utility**
Helper classes and interfaces:
- `BusManagementInterface.java`: Interface defining methods for ticket management.
- `TicketNoGenerator.java`: Utility class to generate unique ticket numbers.

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/BusTicketManagementSystem.git
