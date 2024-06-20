# CPU Scheduler
Made for ACM Open Projects Summer of 2024

## Project Description
Operating systems play a crucial role in managing computer resources efficiently, with process scheduling being a fundamental component. A CPU scheduler is responsible for managing the execution of processes. It decides which process should utilize the CPU and for how long, ensuring efficient resource utilization.

This project implements 7 CPU scheduling algorithms as follows:
* First-Come, First-Served (FCFS)
* Shortest Job First (SJF)
* Shortest Remaining Time First (SRTF)
* Round Robin (RR)
* Priority Scheduling
* Multilevel Queue Scheduling.
* Smart Scheduling
Smart Scheduling chooses the best algorithm depending on the input parameters to minimize the Average Waiting Time of processes and maximize CPU usage.

## Table of Contents
- [Installation](#installation)
- [Technologies Used](#technologies-used)
- [Interaction Flow](#interaction-flow)

## Installation

* Git Clone this Repository
```bash
    https://github.com/ShivanshKasaudhan/CPU-Scheduler.git
```

* Compile the scheduler.cpp file using a compiler with C++ 11 or higher
```bash
    g++ -o scheduler.exe scheduler.cpp
```
* run npm install to install all dependencies
```bash
  npm install my-project
```
* run npm start to run the project
```bash
    npm start
```
## Technologies Used
The CPU Scheduler application leverages modern technologies to deliver a seamless user experience and robust backend processing:

* Electron: A framework for building cross-platform desktop applications using web technologies (HTML, CSS, JavaScript). Electron enables the creation of a responsive and interactive user interface.

* C++: Chosen for its efficiency and low-level system access, C++ forms the backbone of the application's backend, implementing process scheduling algorithms and performance metrics calculations.

* IPC (Inter-Process Communication): Facilitates seamless communication between the Electron frontend and C++ backend, enabling real-time data exchange and synchronization for interactive visualization.
## Interaction Flow
The interaction flow between the frontend and backend of the CPU Scheduler application is as follows:

1. The user selects a scheduling algorithm and enters process details (process ID, arrival time, burst time, priority) through the Electron frontend.


2. Upon clicking the "Run Scheduler" button, the frontend sends an IPC message containing the selected algorithm and process details to the backend.

3. The backend receives the IPC message, processes the scheduling request using the specified algorithm, and computes the necessary performance metrics.

4. After completing the scheduling process, the backend sends a response back to the Electron frontend, where the output is formatted to a table.

5. The Electron frontend receives the scheduling results, updates the UI to display the process details, and shows performance metrics such as Completion time, Turnaround time, and Waiting Time for each process with average turnaround time and average waiting time.
## How to use the application
The first look of the application will be like this :
