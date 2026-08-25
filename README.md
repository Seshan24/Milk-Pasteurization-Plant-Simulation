# Milk Pasteurization Plant Simulation

## Description

A Python-based simulation of an automated milk pasteurization process, covering storage, tank control, heating, pasteurization, cooling, and packaging.

## Features

- Storage tank temperature monitoring
- Milk level sensor control
- Balance tank level control
- Inlet valve regulation
- Heating flow-rate calculation
- Pasteurization at 72°C
- 15-second holding process
- Cooling to 4°C
- Packaging simulation
- Safety condition monitoring

## Process Flow

```text
Storage Tank
     ↓
Balance Tank
     ↓
Heating
     ↓
Holding Tube
     ↓
Cooling
     ↓
Packaging
```

## Requirements

- Python 3.x
- Jupyter Notebook / Google Colab

## How to Run

1. Open `Untitled6.ipynb`.
2. Run the Python code.
3. Monitor the output for each process stage.
4. The simulation completes after successful cooling and packaging.

## Main Parameters

- Target pasteurization temperature: **72°C**
- Holding time: **15 seconds**
- Final cooling temperature: **4°C**
- Milk flow rate: **2.5 kg/s**
- Water inlet temperature: **85°C**
- Water outlet temperature: **75°C**

## Project Objective

To demonstrate basic industrial process-control concepts using Python, including sensor logic, temperature regulation, calculations, safety checks, timing, and sequential automation.

## Note

This project is an educational simulation and is not intended for controlling a real industrial milk pasteurization plant.