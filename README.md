# Siemens TIA Portal: Data Handling & Memory Mapping (Proof of Concept)

## 🎯 Project Objective

This technical Proof of Concept (PoC) is designed to demonstrate a solid understanding of fundamental PLC programming principles in Siemens TIA Portal. Rather than simulating a complete industrial process, the project focuses on data type management, signal processing, and memory allocation techniques commonly used in industrial automation.

## 💡 Core Concept

The project is based on a simple conveyor-belt scenario in which items are counted and their total weight is calculated.

Although the application itself is intentionally simple, it serves as a practical environment for demonstrating the following key PLC programming skills:

1. **Edge Detection:** Using Positive Edge Triggers (`P_TRIG`) to capture sensor pulses accurately and prevent false counting.
2. **Data Type Conversion:** Converting integer data (`INT`) to floating-point data (`REAL`) using the `CONVERT` block to enable mixed-type mathematical operations.
3. **Memory Safety:** Explicitly assigning memory addresses (`%MW20`, `%MD24`, `%MD28`) to prevent memory overlap, a common issue in S7-1200 and S7-1500 controllers.

## 🛠️ Included Components

* Ladder Logic (`OB1`) organized into three clearly structured networks with professional comments.
* A pre-configured Watch Table (`Production_Monitoring`) for simulation using S7-PLCSIM and real-time monitoring of data changes.
