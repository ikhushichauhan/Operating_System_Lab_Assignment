#  Operating System Lab Assignments (ENCA252)

##  Overview

This repository contains lab assignments for **Fundamentals of Operating System (ENCA252)** as part of **BCA (AI & DS)**.

It includes implementation of:

* CPU Scheduling Algorithms (FCFS & SJF)
* Banker’s Algorithm (Deadlock Avoidance)

 Assignment References:

* CPU Scheduling → 
* Banker’s Algorithm → 

---

#  Assignment 1: CPU Scheduling (FCFS & SJF)

##  Objectives

* Understand CPU scheduling concepts
* Implement FCFS and SJF algorithms
* Calculate CT, TAT, WT
* Compare algorithm performance

---

##  Features

###  Process Creation

* Created `Process` class with:

  * PID
  * Arrival Time
  * Burst Time

###  FCFS Scheduling

* Executes processes in order of arrival
* Calculates:

  * Completion Time (CT)
  * Turnaround Time (TAT)
  * Waiting Time (WT)

###  SJF Scheduling

* Selects process with shortest burst time
* Improves average waiting time

###  Gantt Chart

* Displays execution order of processes

###  Performance Analysis

* Calculates average WT & TAT
* Compares FCFS vs SJF

---

##  Sample Output

### FCFS

```
PID   AT   BT   CT   TAT   WT
1     0    5    5    5     0
2     1    2    7    6     4
...
```

### SJF

```
PID   AT   BT   CT   TAT   WT
1     0    5    5    5     0
4     3    1    6    3     2
...
```

---

##  Conclusion

* **SJF** gives better performance (lower waiting time)
* **FCFS** is simple but less efficient

---

#  Assignment 2: Banker’s Algorithm

##  Objectives

* Understand deadlock avoidance
* Implement Banker’s Algorithm
* Determine safe/unsafe state
* Find safe execution sequence

---

##  Features

###  System Input

* Number of processes & resources
* Allocation Matrix
* Maximum Matrix
* Available Resources

###  Need Matrix

```
Need = Maximum - Allocation
```

###  Safety Algorithm

* Checks if system is in safe state
* Uses Work & Finish arrays

###  Safe Sequence

* Generates safe execution order

###  Result Analysis

* Displays:

  * SAFE / UNSAFE state
  * Safe sequence

---

##  Sample Output

```
System is in SAFE STATE
Safe Sequence: P1 → P2 → P0
```

---

##  Conclusion

* Banker’s Algorithm prevents deadlock
* Ensures system remains in safe state

---

#  How to Run

```bash
# Run CPU Scheduling
python main.py

# Run Banker's Algorithm
python bankers.py
```

---

#  Author

**Khushi Chauhan**
BCA (AI & DS)
K.R. Mangalam University

---

#  Note

This project is created for academic purposes as part of OS Lab assignments.
