# 🔲 Logic Gates — CMOS VLSI (Full Custom)

This `combinational` repository contains full-custom layouts and simulations of basic logic gates: `NOT`, `NAND`, `NOR`, 
`AND`, `OR`, `XOR`, and a simple `2:1 multiplexer`.

Each gate has its own folder with:
- Custom layout in Magic VLSI
- Schematic in Xschem
- LVS checks with Netgen
- SPICE simulation using ngspice
- Parasitic-aware analysis

---

## 🛠 Tools Used

| Tool        | Purpose                                 |
|-------------|-----------------------------------------|
| Magic VLSI  | Physical layout and netlist extraction  |
| ngspice     | Transient simulation of SPICE netlists  |
| Xschem      | Schematic capture and SPICE export      |
| netgen      | LVS comparison between layout and schematic |

---


---

## 🧠 Theory: Static CMOS Logic

In static CMOS logic, any function can be implemented using a pull-up network (PUN) and a pull-down network (PDN). Each consists of PMOS and NMOS transistors arranged complementarily.

This ensures:
- Output is always connected to either VDD or GND
- No direct current path between power and ground
- Low static power dissipation
- High noise margins and fast switching

---

## 💡 Example: Inverter Gate

### Transistor-Level Schematic

<p align="center">
  <img src="./inverter/inverter_schematic.png" width="600" />
</p>
<p align="center"><em>Single-input NOT schematic (Xschem)</em></p>

### Layout (Magic VLSI)

<p align="center">
  <img src="./inverter/inverter_vlsilayout.png" width="600" />
</p>
<p align="center"><em>Magic VLSI layout (with DRC clean)</em></p>

---


## ✅ Takeaways
- Learned how to extract parasitics and simulate post-layout
- Understand layouts of basic logic gates

---


## 🙌 Closing Notes
This repo is for students, researchers, and hobbyists learning VLSI using open tools.
Feel free to fork, open issues, or contribute new gate implementations!

---
