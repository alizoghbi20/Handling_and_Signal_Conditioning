# Siemens TIA Portal: Data Handling & Memory Mapping (Proof of Concept)

## 🎯 Project Objective
This is a technical Proof of Concept (PoC). The primary goal is not to simulate a full industrial plant, but rather to demonstrate a solid understanding of fundamental PLC programming principles in Siemens TIA Portal, specifically focusing on data type management and memory allocation.

## 💡 The Core Concept
The project uses a simple theoretical scenario: counting items on a conveyor belt and calculating their total weight. 
While the scenario is basic, it serves as a testing ground to apply the following critical skills:
1. **Signal Catching:** Using Positive Edge Triggers (`P_TRIG`) to capture physical sensor pulses accurately without false counts.
2. **Data Type Casting:** Converting integer data (`Int`) to floating-point data (`Real`) using the `CONVERT` block to allow for mixed-type mathematical operations.
3. **Memory Safety:** Explicitly mapping memory addresses (`%MW20`, `%MD24`, `%MD28`) to completely prevent Memory Overlap—a common error in S7-1200/1500 controllers.

## 🛠️ What is Included?
* Ladder Logic (`OB1`) divided into three clear networks with professional comments.
* A pre-configured Watch Table (`Production_Monitoring`) to run the simulation via S7-PLCSIM and observe the data transitions live.
