# Tutorial 12: Exception Handling in Java

This repository contains Java implementations for **Tutorial 12** of the Object-Oriented Programming (OOP) course. The tutorial focuses on custom exception handling using **Checked** and **Unchecked Custom Exceptions**.

---

## 📌 Project Overview

| Details | Description |
| :--- | :--- |
| **Course Name** | Object Oriented Programming |
| **Course Code** | 24SJPBCST304 |
| **Academic Year** | 2026-2027 |
| **Topic** | Exception Handling (Custom Exceptions) |
| **IDE** | Eclipse Java IDE |

---

## 📝 Questions & Program Descriptions

### Question 1: Invalid Number Exception (`InvalidNumberException`)
* **Goal:** Create a user-defined checked exception `InvalidNumberException` to process $N$ positive numbers, filter out non-positive inputs (negative or zero), and calculate the sum and average.
* **Key Components:**
  * **Custom Exception Class**: `InvalidNumberException extends Exception`
  * **Main Class**: Accepts $N$ user inputs, throws custom exception for values $\le 0$, handles exceptions using `try-catch`, and computes the sum and average of positive values.

---

### Question 2: Hotel Room Reservation System (`InvalidReservationException`)
* **Goal:** Create a custom exception `InvalidReservationException` to manage reservation requests for hotel rooms.
* **Key Components:**
  * **Custom Exception Class**: `InvalidReservationException extends Exception`
  * **Class `HotelRoom`**: Manages available room slots and validates requested reservations.
  * **Validation Rule**: Throws exception if requested slots are $\le 0$ or exceed available capacity.

---

### Question 3: Student Score Validator (`InvalidScoreException`)
* **Goal:** Implement an **unchecked custom exception** to validate student scores.
* **Key Components:**
  * **Custom Exception Class**: `InvalidScoreException extends RuntimeException`
  * **Class `Student`**: Validates whether the score falls within the valid range ($0 \le \text{score} \le 100$).
  * **Validation Rule**: Throws exception if score is less than $0$ or greater than $100$.

---

## 🚀 How to Run in Eclipse

1. **Open Eclipse** and select your workspace.
2. Create a new Java Project:
   * **File** ➔ **New** ➔ **Java Project**
   * Project Name: `Tutorial12`
3. Add source files:
   * Right-click `src` ➔ **New** ➔ **Class**.
   * Create `Question1.java` and paste the code for Question 1.
   * Create `Question2.java` and paste the code for Question 2.
   * Create `Question3.java` and paste the code for Question 3.
4. **Run the Programs**:
   * Open any of the files and press `Ctrl + F11` (or click the green **Run** button).
   * Enter input values in the **Console window** at the bottom.

---

## 🖥 Sample Execution Output

### Question 1 Output Example:
```text
Enter 5 Numbers
12
-10
14
-15
16
Numbers are
12
invalid Number-10
14
invalid Number-15
16

sum of the positive numbers are: 42
Average of these numbers: 14.0
