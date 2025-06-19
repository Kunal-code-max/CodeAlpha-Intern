# CodeAlpha-Intern
# Java Mini‑Projects

This repository contains two small, self‑contained Java console applications created as learning exercises.

| Task  | File                        | Description                                                                                          |
| ----- | --------------------------- | ---------------------------------------------------------------------------------------------------- |
| **1** | `StudentGradeManager.java`  | Manage student grades: add students, list scores, and compute statistics (average, highest, lowest). |
| **2** | `StockTradingPlatform.java` | Simulate a very basic stock‑trading environment with buy/sell operations and portfolio tracking.     |

Both programs are written for **JDK 17+** (but will compile on JDK 11 as well). They have **no external dependencies** — just compile and run.

---

## 1  Student Grade Manager

### Features

* Add students with numeric scores (0‑100)
* View a **summary report** that lists every student alongside

  * Average score
  * Highest score
  * Lowest score
* Input validation on menu options and numeric ranges
* Easily extendible (e.g. edit/delete students, save to file)

### Compile & Run

```bash
javac StudentGradeManager.java
java  StudentGradeManager
```

### Usage Snapshot

```
========================================
        Student Grade Manager v1.0
========================================

1. Add Student & Score
2. Show Summary Report
3. Exit

Choose an option: 1
Enter student name: Alice
Enter score (0-100): 93
Added Alice with score 93.00
```

---

## 2  Stock Trading Platform

### Features

* Built‑in market data for AAPL, GOOG, TSLA, AMZN (prices hard‑coded)
* **Buy** and **sell** shares with automatic cash/holding updates
* View a live **portfolio report** (share count × current price)
* Easily extend to multiple users, price‑fluctuation simulation, or persistent storage

### Compile & Run

```bash
javac StockTradingPlatform.java
java  StockTradingPlatform
```

### Usage Snapshot

```
1. View Market
2. Buy Stock
3. Sell Stock
4. View Portfolio
5. Exit
Choose an option: 1

--- Market Data ---
AAPL (Apple Inc.): $172.3
GOOG (Alphabet Inc.): $2835.0
TSLA (Tesla Inc.): $700.0
AMZN (Amazon.com Inc.): $3300.0
```

> **Tip:** Start with the `$10,000` default cash balance, buy a few shares, then view your portfolio to see the running valuations.

---

## Extending the Projects

Both programs focus on core logic and are deliberately concise. Potential improvements:

* **StudentGradeManager**

  * Persist student data to a CSV or database
  * Letter‑grade mapping and histogram charting
  * GUI (Swing or JavaFX)
* **StockTradingPlatform**

  * Real‑time price simulation using a background thread
  * Multi‑user support with login credentials
  * JSON/YAML persistence of portfolios
  * Simple REST API or web UI (Spring Boot)

Feel free to fork and enhance as you learn — happy coding! 🎉
