# IIT Patna - EC3102: VLSI Design Lab Coursework (Cadence Virtuoso)

## 📌 Course Overview
This repository contains lab experiments and simulation reports completed as part of **EC3102: VLSI Design Lab** at the **Indian Institute of Technology Patna (IIT Patna)** during the 5th semester[cite: 5]. All transistor-level designs, schematic captures, and transient/DC analyses were performed using **Cadence Virtuoso** via Xming/PuTTY[cite: 7].

* **Student Name:** Saksham Srivastava[cite: 5]
* **Roll No:** 2301EC56[cite: 5]
* **Group:** Tuesday Group[cite: 5]

---

## 📂 Laboratory Experiments Included

### Experiment 01: MOSFET DC Characteristics ($I_D\text{ vs }V_{DS}$ & $I_D\text{ vs }V_{GS}$)
* **Aim:** Study and plot current-voltage ($I\text{-}V$) output and transfer characteristics for NMOS and PMOS transistors[cite: 7].
* **Simulations Performed:** 
  * Output characteristics ($I_D$ vs $V_{DS}$) at stepped constant values of $V_{GS}$[cite: 7].
  * Transfer characteristics ($I_D$ vs $V_{GS}$) at constant $V_{DS}$[cite: 7].

### Experiment 02: Pass-Transistor Logic (PTL) Gates
* **Aim:** Design and simulate various logic gates using Pass-Transistor Logic and evaluate their functionality and voltage drop limitations[cite: 9].
* **Implementations:** NMOS/PMOS pass transistors, NAND, NOR, AND, OR, XOR, and XNOR gates using PTL[cite: 10, 11].

### Experiment 03: CMOS Inverter, NAND, and NOR Analysis
* **Aim:** Design universal gates (NAND and NOR) and a CMOS Inverter; perform DC, transient, and power analyses[cite: 14, 15].
* **Key Metrics Extracted:**
  * **DC Analysis & Noise Margins:** Evaluated $NM_L$ and $NM_H$ from voltage transfer characteristics (VTC)[cite: 18].
  * **Transistor Sizing ($W_n$ vs $W_p$):** Tested CMOS inverter performance across different sizing ratios ($W_n = W_p$, $W_n = 2W_p$, $W_n = 0.5W_p$)[cite: 15, 16].
  * **Propagation Delay & Switching Speed:** Measured $T_{PLH}$ and $T_{PHL}$ across best and worst input patterns, computing maximum switching frequencies ($F_{max} > 1.2\text{ GHz}$)[cite: 18].
  * **Power Consumption:** Estimated static and dynamic power dissipation at $100\text{ MHz}$ and $500\text{ MHz}$ operating frequencies[cite: 18].

### Experiment 04: Custom Cell Library & "Bob's Designs" Optimization
* **Aim:** Create hierarchical symbols for fundamental logic gates (NAND, NOR, AND, OR, XOR, XNOR) and evaluate two competing complex logic architectures ("Bob's Design 1" vs. "Bob's Design 2")[cite: 19].
* **Comparative Results:**
  * **Bob's Design #1:** Critical path delay $T_p = 0.164\text{ ns}$, Maximum switching speed $F_{max} = 6.097\text{ GHz}$, Average Power = $171.7\text{ }\mu\text{W}$[cite: 23].
  * **Bob's Design #2:** Critical path delay $T_p = 0.361\text{ ns}$, Maximum switching speed $F_{max} = 2.77\text{ GHz}$, Average Power = $221.6\text{ }\mu\text{W}$[cite: 23].
* **Conclusion:** Design #1 was selected as optimal due to its superior speed and lower power consumption resulting from simpler single-gate logic on critical outputs[cite: 23].

---

## 🛠️ Tools & Environment
* **EDA Tool:** Cadence Virtuoso (Spectre Simulator)[cite: 7, 23]
* **Remote Access:** PuTTY, Xming[cite: 7]
* **Technology Node:** Sub-micron CMOS process models

---

## 🚀 How to Use This Repository
1. Open your Cadence Virtuoso workspace.
2. Import the netlists or schematic views corresponding to each experiment folder.
3. Run ADE (Analog Design Environment) simulations to reproduce DC sweep, transient, and power measurements.
