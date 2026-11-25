🎫 Simple Ticket Queue System

A Java-Based Customer Ticket Management System Using Data Structures & Algorithms

<p align="center">
  <b>Organize. Manage. Serve. Efficiently.</b>
</p><p align="center">
  <img src="https://img.shields.io/badge/Language-Java-orange?style=for-the-badge&logo=openjdk" />
  <img src="https://img.shields.io/badge/DSA-Queue-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Data%20Structure-Array-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Linked%20List-Implemented-purple?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" />
</p>---

📌 Overview

The Simple Ticket Queue System is a menu-driven Java application developed as a Data Structures and Algorithms (DSA) academic project.

The application provides an organized way to manage customer service requests through a ticket-based system. Every customer receives a unique ticket ID, and requests are processed according to their arrival order using the FIFO (First In, First Out) principle.

The project demonstrates the practical implementation of three fundamental data structures:

- Array – Stores and manages ticket records.
- Queue – Maintains the waiting line and ensures FIFO processing.
- Singly Linked List – Maintains the history of served and cancelled tickets.

🎯 Project Objectives

- Develop a structured ticket management system using Java.
- Implement FIFO-based customer service.
- Generate unique ticket IDs for customers.
- Maintain and search customer ticket records.
- Track served and cancelled tickets.
- Understand the practical application of fundamental DSA concepts.

✨ Features

Feature| Description
🎫 Generate Ticket| Creates a new ticket with a unique ID.
📋 View Waiting Queue| Displays all customers waiting for service.
⚡ Serve Next Customer| Serves the earliest registered customer.
🔍 Search Ticket| Searches tickets using their unique ID.
❌ Cancel Ticket| Cancels a ticket that is still waiting.
📑 Display All Tickets| Displays all generated ticket records.
📚 Ticket History| Displays served and cancelled ticket records.
📊 Waiting Count| Shows the number of customers waiting.

🧠 Data Structures Used

1. Array

An array stores all generated ticket records.

Implementation:

Ticket[] ticketRecords = new Ticket[1000];

Purpose:

- Maintains all ticket records.
- Provides indexed access.
- Supports searching and displaying tickets.

2. Queue

The Queue interface with "ArrayDeque" manages customers waiting for service.

Implementation:

Queue<Ticket> waitingQueue = new ArrayDeque<>();

FIFO Principle:

First In → First Out

Important operations:

Operation| Method
Insert ticket| "offer()"
Serve next customer| "poll()"
View next customer| "peek()"
Check waiting count| "size()"

3. Singly Linked List

A custom singly linked list maintains the history of served and cancelled tickets.

Node structure:

static class Node {
    Ticket ticket;
    Node next;
}

Each node contains ticket information and a reference to the next node.

Purpose:

- Maintains ticket history dynamically.
- Supports insertion at the tail.
- Allows sequential traversal of history records.

⚙️ System Workflow

             START
               |
               ▼
       Initialize System
               |
               ▼
          Display Menu
               |
               ▼
        Select Operation
               |
       ┌───────┼────────┐
       ▼       ▼        ▼
    Generate  Serve    Search
     Ticket  Customer  Ticket
       |       |        |
       ▼       ▼        ▼
    Add to   Remove   Find in
    Array    from     Array
             Queue
               |
               ▼
       Update Ticket Status
               |
               ▼
       Update History List
               |
               ▼
         Return to Menu
               |
               ▼
              EXIT

📂 Project Structure

Simple-Ticket-Queue-System/
│
├── SimpleTicketQueueSystem.java
│
├── README.md
│
└── screenshots/
    ├── main-menu.png
    ├── ticket-generation.png
    ├── waiting-queue.png
    └── ticket-history.png

🚀 Getting Started

Prerequisites

- Java Development Kit (JDK 17 or later recommended).
- VS Code, IntelliJ IDEA or Eclipse.
- Basic knowledge of Java programming.

Installation

1. Clone the repository

git clone https://github.com/YOUR-USERNAME/Simple-Ticket-Queue-System.git

2. Navigate to the project directory

cd Simple-Ticket-Queue-System

3. Compile the Java program

javac SimpleTicketQueueSystem.java

4. Execute the application

java SimpleTicketQueueSystem

📈 Time Complexity Analysis

Let:

- "n" = Total generated tickets
- "w" = Number of waiting tickets
- "h" = Number of history entries

Operation| Time Complexity
Generate Ticket| O(1) amortized
Serve Next Customer| O(1)
Search Ticket| O(n)
View Waiting Queue| O(w)
Cancel Ticket| O(n + w)
Display All Tickets| O(n)
Display History| O(h)
Waiting Count| O(1)

🔮 Future Improvements

Some possible enhancements for future versions:

- Database integration for permanent ticket storage.
- Graphical User Interface (GUI).
- Multiple service counters.
- Priority-based ticket management.
- Customer and administrator authentication.
- Ticket generation timestamps.
- Estimated customer waiting time.

🎓 Academic Project Information

Detail| Information
Project Name| Simple Ticket Queue System
Student Name| Manjeet Kumar
ERP ID| RU-25-11746
Course| B.Tech Computer Science & Engineering
Subject| Data Structures and Algorithms
Programming Language| Java
University| Rungta International Skills University
Project Guide| Ms. Naina Singh
Academic Session| 2026–27

👨‍💻 Author

Manjeet Kumar

B.Tech CSE | AI & ML

- GitHub: "@PERO-99" (https://github.com/PERO-99)

---

⭐ Acknowledgement

This project was developed as part of the Data Structures and Algorithms coursework to understand and demonstrate the practical implementation of arrays, queues and linked lists in Java.

If you find this project useful, consider giving the repository a ⭐!

<p align="center">
  Made with ☕ and Java by Manjeet Kumar
</p>
