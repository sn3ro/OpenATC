# OpenATC

**Open-source modular automatic tool changer (ATC) for hobby CNC routers, using spindle inertia for reliable collet tightening.**

OpenATC is a DIY automatic tool-change system designed to be easy to build, easy to retrofit, and fully open for modification.  
The system uses a unique **inertia-based tightening mechanism**: instead of relying on weak cams or springs, the spindle’s rotational inertia is used to lock the ER20 collet nut with a controlled, sudden deceleration.

This repository contains all CAD files, 3D-printable parts, LinuxCNC configuration examples, documentation, and sourcing information required to build your own OpenATC.

---

## ✨ Features

- 🧩 **Modular tool holders** – add as many as you like  
- 🔄 **Automatic tightening** using spindle inertia  
- 🧱 **3D-printable** components (designed for PETG)  
- 🛠 **Easy to build** with common tools and off-the-shelf fasteners  
- 💻 **LinuxCNC-compatible** with example macros included  
- 🌍 **Fully open-source (MIT)** – build, modify, and use freely  

---

## ⚙️ How It Works

Commercial hobby-grade ATC systems often rely on limited mechanical leverage to tighten the collet nut.  
OpenATC instead uses:

- A standard **ER20 2.2 kW spindle**, typically at **~700 rpm**  
- A mechanism that brings the nut to a **controlled stop**  
- The spindle’s **rotational inertia** to generate tightening torque

This results in approximately **8 Nm** of tightening torque

The design is intended to be safe, simple, and replicable with common hobby CNC equipment.

---

## 📁 Repository Structure

OpenATC/
├─ hardware/
│ ├─ cad/ # Fusion 360 source files, STEP exports
│ ├─ stl/ # 3D-printable components
│ ├─ drawings/ # Optional technical drawings
│ └─ bom/ # Bill of materials + sourcing info
│ ├─ openatc_bom.csv
│ ├─ alternates.md
│ └─ sourcing-guide.md
├─ cnc-config/
│ ├─ linuxcnc/ # Example M6 remap, macros, HAL snippets
│ └─ other/ # Reserved for future Mach/GRBL examples
├─ docs/
│ ├─ assembly.md
│ ├─ setup.md
│ ├─ theory.md
│ ├─ safety.md
│ └─ faq.md
├─ media/
│ ├─ photos/
│ ├─ renders/
│ └─ animations/
└─ examples/
├─ gcode/
└─ projects/


---

## 📦 Bill of Materials (BOM)

OpenATC uses a small number of purchased components such as:

- Compression springs  
- Standard metric screws  
- Hardened washers  

The full bill of materials, along with alternates and sourcing guidance, is located in:  

TBC


These parts are intentionally generic so builders can source them locally.

---

## 🛠 Getting Started

1. **Print the STL parts** from `hardware/stl/`  
2. **Source the bought-in components** listed in the BOM  
3. **Assemble the ATC** using `docs/assembly.md`  
4. **Install and configure your system** using the examples in `cnc-config/linuxcnc/`  
5. **Test tool changes** with the example G-code in `examples/gcode/`

---

## 🔒 Safety Notice

OpenATC intentionally uses **controlled deceleration of a rotating spindle** to tighten the collet nut.

Before operating:

- Always test without tooling first  
- Verify spindle braking and acceleration settings  
- Ensure guarding is in place during testing  
- Use appropriate PPE  
- Confirm that all 3D-printed parts are structurally sound  

You build and use this system **at your own risk**.

---

## 🤝 Contributing

Contributions are welcome!  
You can help by:

- Testing the design and reporting issues  
- Improving documentation  
- Submitting CAD/model refinements  
- Adding controller configuration examples  
- Suggesting improvements or new tool holder types  

OpenATC is intended to evolve through community input.

---

## 📜 License

This project is licensed under the **MIT License**.  
You are free to use, modify, and redistribute the design for personal or commercial use.  
See the `LICENSE` file for full terms.

---

## 📧 Contact / Discussion

If you have questions, ideas, or build results, feel free to:

- Open a GitHub Issue  
- Start a Discussion (if enabled)  
- Share your build photos or improvements  

OpenATC is a community-driven open hardware project — enjoy building!





