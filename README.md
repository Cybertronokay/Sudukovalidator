# 🧩 Sudoku Validator – Software Engineering Project

## 📘 Project Overview

**Sudoku Validator** is a full-stack Software Engineering mini project that validates a 9x9 Sudoku grid submitted by a user through a web interface. The grid is passed to a Python Flask API, which writes the input to a file and delegates the actual validation logic to a C++ program.

This project follows **modular design**, uses **file-based inter-process communication**, and integrates a **multithreaded backend** to enhance performance and efficiency.

---

## 💡 Why Multithreading?

To improve the efficiency of validation, the C++ backend uses **multithreading** to **parallelize** the following tasks:

- ✅ Row validation
- ✅ Column validation
- ✅ 3×3 subgrid validation

Each of these is handled in a separate thread using C++'s `<thread>` library. This approach reduces execution time and demonstrates how concurrency improves system performance in real-world software.

---

## 🔧 Technologies Used

| Component     | Technology         |
|---------------|--------------------|
| Frontend      | HTML, JavaScript   |
| Backend API   | Python (Flask)     |
| Core Logic    | C++ (with Threads) |
| Communication | JSON, File I/O     |

---

## 🧱 System Architecture

