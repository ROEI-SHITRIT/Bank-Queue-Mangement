# Bank-Queue-Management

## Overview
This project is a bachelor's degree assignment in the Object-Oriented Java course. It is designed to develop and assess skills in the following areas:

- Object-oriented design with multiple classes.
- Data structures.
- Java programming.
- Multithreading programming.
- Synchronized threads.
- Problem-solving.
- Debugging.

The project simulates a bank queue, including bank tellers, customers, a bank clock, and a system sampler. The goal is to manage the queue efficiently by assigning available tellers to customers as they arrive.

## Features:

### Bank
- Activates a clock to signal the beginning and end of the working day.
- Creates and manages tellers according to a predefined number.
- Initializes a sampler to monitor the system.
- Generates customers at a predetermined rate and initiates their operations.
- Configurable parameters: working day duration, number of tellers, customer arrival rate, sampling cycle, and queue management.

### Clock
- Controls the working day's schedule.
- Announces when the bank opens and closes.

### Teller
- Serves customers in order from the queue.
- Processes each customer for a predefined service duration.
- Calls the next customer once the previous one is done.
- Works continuously throughout the day.
- Stops working only after all customers in the queue are served at the end of the day.
- Reports the total number of customers served at the end of the day.

### Customer
- Waits in the queue until assigned to a teller.
- Undergoes three states:
  - **Waiting**
  - **Receiving service**
  - **Done**
- Has a predefined service time.

### Sampler
- Monitors and logs system status at predefined intervals.
- Provides information on which teller is serving which customer at any given time.

## Installation and Usage
### Prerequisites
- Java Development Kit

UML Diagram:
![image](https://github.com/user-attachments/assets/c7766ad4-b50c-47b4-a878-2adc2d91b743)

## Challenges during the project:


-Synchronizing threads to ensure all components work correctly together.

-Coordinating between the simulator and the bank clock to ensure proper termination of operations.

-Handling edge cases such as variable service times and unexpected customer surges.

-Managing communication between tellers and customers without causing deadlocks or unnecessary delays.

-Ensuring accurate sampling by the sampler to reflect the real system state.

-Debugging and fixing issues caused by shared resource access between multiple threads.

