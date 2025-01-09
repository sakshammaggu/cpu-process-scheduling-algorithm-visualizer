# CPU Process Scheduling Algorithms Visualizer

A comprehensive visualizer for CPU scheduling algorithms, implemented in C++ with SDL2 for visualizations. The project supports various scheduling algorithms like FCFS, SJF, LJF, LRTF, and Round Robin, and provides users with intuitive 2D representations such as Gantt charts and process queues.

---

## 📋 Table of Contents
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Folder Structure](#folder-structure)
- [Installation](#installation)
- [Build and Run](#build-and-run)
- [Commands for Visualization](#commands-for-visualization)

---

## ✨ Features
- Supports multiple CPU scheduling algorithms:
  - First Come First Serve (FCFS)
  - Shortest Job First (SJF)
  - Longest Job First (LJF)
  - Longest Remaining Time First (LRTF)
  - Round Robin (RR)
- Visualizes algorithms using SDL2:
  - Gantt Charts
  - Process Queues
- Modular folder structure for easy maintenance.

---

## 💻 Tech Stack
- **Programming Language:** C++
- **Build Tools:** MinGW, CMake, Makefile
- **Visualization Framework:** SDL2

---

## 📂 Folder Structure
```
CpuVis
├── algorithms
│   ├── firstComeFirstServe
│   │   ├── firstComeFirstServe.cpp
│   │   ├── firstComeFirstServeVisualizer.cpp
│   │   └── firstComeFirstServe.h
│   ├── longestJobFirst
│   ├── longestRemainingTimeFirst
│   ├── roundRobin
│   └── shortestJobFirst
├── build
├── include
├── src
│   └── main.cpp
├── SDL2
│   ├── include
│   ├── lib
├── CMakeLists.txt
├── Makefile
└── README.md
```

---

## 🔧 Installation

### 1. Prerequisites
- **C++ Compiler:** MinGW (for Windows)
- **Build Tools:** CMake, Makefile
- **SDL2 Library:** Download and set up SDL2 as follows:

### 2. Setting up SDL2
1. Download SDL2 from [SDL2 Downloads](https://www.libsdl.org/download-2.0.php).
2. Extract the files and place them in the `SDL2` folder.
   - Include files in `SDL2/include`
   - Library files in `SDL2/lib`

### 3. Clone the Repository
```bash
git clone https://github.com/yourusername/CpuVis.git
cd CpuVis
```

---

## 🛠️ Build and Run

### 1. Build using CMake
```bash
mkdir build
cd build
cmake ..
make
```

### 2. Run the Application
```bash
./CpuVis
```

---

## 🖼️ Commands for Visualization
Use the following commands to compile and visualize different scheduling algorithms:

### FCFS (First Come First Serve)
```bash
g++ -I SDL2/include -L SDL2/lib -o fcfs algorithms/firstComeFirstServe/firstComeFirstServeVisualizer.cpp -lmingw32 -lSDL2main -lSDL2 -lSDL2_ttf
```
### LJF (Longest Job First)
```bash
g++ -I SDL2/include -L SDL2/lib -o ljf algorithms/longestJobFirst/ljfVisualizer.cpp -lmingw32 -lSDL2main -lSDL2 -lSDL2_ttf
```
### LRTF (Longest Remaining Time First)
```bash
g++ -I SDL2/include -L SDL2/lib -o lrtf algorithms/longestRemainingTimeFirst/lrtfVisualizer.cpp -lmingw32 -lSDL2main -lSDL2 -lSDL2_ttf
```
### RR (Round Robin)
```bash
g++ -I SDL2/include -L SDL2/lib -o rr algorithms/roundRobin/rrVisualizer.cpp -lmingw32 -lSDL2main -lSDL2 -lSDL2_ttf
```
### SJF (Shortest Job First)
```bash
g++ -I SDL2/include -L SDL2/lib -o sjf algorithms/shortestJobFirst/sjfVisualizer.cpp -lmingw32 -lSDL2main -lSDL2 -lSDL2_ttf
```

---
