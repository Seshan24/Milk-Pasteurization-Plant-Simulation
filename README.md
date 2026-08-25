# README.md

````
# 🥛 Milk Pasteurization Plant Simulation

An interactive **Milk Pasteurization Plant Simulation** developed using **Python and Jupyter Notebook**.

This project simulates the main stages of a milk pasteurization process with an interactive control panel, process monitoring, temperature controls, flow-rate controls, and visual status indicators.

---

## 🚀 Features

- 🛢️ Storage Tank monitoring
- 🔄 Balance Tank control
- 🔥 Milk heating process
- ⏱️ 15-second pasteurization holding process
- ❄️ Milk cooling process
- 📦 Packaging stage
- 🌡️ Temperature controls
- 💧 Milk flow-rate control
- ⚙️ Automatic hot-water flow calculation
- 📊 Interactive progress indicators
- ▶️ Full simulation button
- ↺ Reset button
- ✅ Process status monitoring
- ⚠️ Warning and error indicators
- 🎨 Interactive dashboard-style UI

---

## 🔄 Process Flow

```text
┌─────────────────┐
│  Storage Tank   │
└────────┬────────┘
         ↓
┌─────────────────┐
│  Balance Tank   │
└────────┬────────┘
         ↓
┌─────────────────┐
│     Heater      │
└────────┬────────┘
         ↓
┌─────────────────┐
│  Holding Tube   │
│    15 Seconds   │
└────────┬────────┘
         ↓
┌─────────────────┐
│     Cooling     │
└────────┬────────┘
         ↓
┌─────────────────┐
│    Packaging    │
└─────────────────┘
````

---

## 🧪 Simulation Stages

### 1. Storage Tank

The storage tank monitors:

* Milk temperature
* Milk level
* Propeller motor status
* Cooling status

If the milk temperature is above the defined safe condition, the simulation indicates that the cooling system is activated.

---

### 2. Balance Tank

The balance tank controls the milk inlet according to the tank level.

**Low Level**

```text
Inlet Valve → OPEN
```

**Full Level**

```text
Inlet Valve → CLOSED
```

This prevents the tank from overflowing.

---

### 3. Heater

The heater increases the milk temperature toward the pasteurization target.

The simulation uses:

* Milk flow rate
* Milk inlet temperature
* Hot-water inlet temperature
* Hot-water outlet temperature
* Specific heat capacity

to calculate the required hot-water flow.

The default pasteurization target is:

```text
72°C
```

---

### 4. Holding Tube

When the milk reaches the required pasteurization temperature, the holding process starts.

```text
Pasteurization Temperature = 72°C
Holding Time = 15 seconds
```

A progress indicator displays the holding process.

If the required temperature is not reached, the simulation indicates that the milk should be returned to the heating stage.

---

### 5. Cooling

After the holding stage, the milk enters the cooling stage.

The simulation cools the milk toward:

```text
4°C
```

A temperature progress indicator shows the cooling process.

---

### 6. Packaging

After the milk reaches the required cooling temperature, it is transferred to the packaging stage.

The simulation then displays:

```text
PROCESS COMPLETED SUCCESSFULLY
```

---

## 🖥️ Control Panel

The interactive UI provides the following controls:

| Control             | Description                    |
| ------------------- | ------------------------------ |
| Milk °C             | Initial milk temperature       |
| Storage             | Storage tank level             |
| Balance             | Balance tank level             |
| Flow kg/s           | Milk flow rate                 |
| Milk inlet          | Milk inlet temperature         |
| Water inlet         | Hot-water inlet temperature    |
| Water outlet        | Hot-water outlet temperature   |
| Run Full Simulation | Starts the complete simulation |
| Reset               | Restores default values        |

---

## 🛠️ Technologies Used

* Python 3
* Jupyter Notebook
* IPyWidgets
* HTML
* CSS

---

## 📦 Installation

Install the required packages:

```bash
pip install ipywidgets notebook
```

---

## ▶️ Running the Project

### Step 1 — Clone or download the project

```bash
git clone <your-repository-url>
cd Milk-Pasteurization-Plant-Simulation
```

### Step 2 — Install dependencies

```bash
pip install ipywidgets notebook
```

### Step 3 — Start Jupyter Notebook

```bash
jupyter notebook
```

### Step 4 — Open the notebook

Open:

```text
Milk_Pasteurization_Plant_UI_Simulation.ipynb
```

### Step 5 — Run the notebook

Run the cells and use the interactive **Plant Control Panel**.

---

## 📁 Project Structure

```text
Milk-Pasteurization-Plant-Simulation/
│
├── Milk_Pasteurization_Plant_UI_Simulation.ipynb
│
└── README.md
```

---

## 🎯 Project Objective

The main objective of this project is to create an interactive educational simulation of a milk pasteurization plant.

The project demonstrates:

* Process automation concepts
* Temperature monitoring
* Tank-level control
* Heating and cooling processes
* Flow-rate calculations
* Process sequencing
* Interactive Python-based UI development

---

## ⚙️ Default Simulation Parameters

```text
Initial Milk Temperature: 5°C
Milk Flow Rate: 2.5 kg/s

Milk Inlet Temperature: 4°C

Hot Water Inlet Temperature: 85°C
Hot Water Outlet Temperature: 75°C

Pasteurization Temperature: 72°C
Holding Time: 15 seconds

Final Cooling Temperature: 4°C
```

---

## ⚠️ Disclaimer

This project is intended for **educational and demonstration purposes only**.

It is not designed to directly control a real industrial milk pasteurization plant.

Real industrial systems require properly validated process parameters, industrial sensors, PLC/SCADA systems, safety controls, food-safety procedures, and regulatory compliance.

---

## 👨‍💻 Author

**Milk Pasteurization Plant Simulation Project**

Developed as an interactive Python/Jupyter-based process simulation.

---

## 📄 License

This project may be used, modified, and extended for educational, academic, and demonstration purposes.

---

```
```
