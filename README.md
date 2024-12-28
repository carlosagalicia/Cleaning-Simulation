# Cleaning Robots Simulation

This project simulates a group of vacuum cleaning agents tasked with cleaning a grid-based room. The room starts with a defined percentage of dirty cells (dirt agents), and the vacuum cleaners navigate the space, cleaning these cells while avoiding collisions with other agents.

## Overview

- **Functionality:** Simulates a room with dirt agents and vacuum cleaning agents. The vacuums clean the room by detecting and moving to dirty cells.
- **Objective:** Test the cleaning efficiency of vacuum agents by measuring the time and steps needed to clean a predefined percentage of dirty cells.

## Key Features

### 1. Agents and Environment
- **Vacuum Cleaner Agents:** Agents move within the room, clean dirty cells, and measure their efficiency based on cleaned and visited cells.
- **Dirt Agents:** Represent dirty cells that the vacuum agents aim to clean.
- **Room Model:** A grid environment where agents operate, represented using Mesa's `SingleGrid`.

### 2. Simulation Process
- **Random Activation:** All agents act in random order within each step.
- **Data Collection:** Tracks the grid's state and performance metrics such as cleaning efficiency and steps required.
- **Visualization:** Displays animations of the cleaning process and collects statistical data for analysis.

### 3. Customization
- Parameters such as room dimensions, the percentage of dirty cells, and the number of vacuum agents can be adjusted to explore different scenarios.

## Languages and Tools Used

### Python
- **Mesa:** For agent-based modeling and simulation.
- **Matplotlib:** For data visualization and animations.
- **Seaborn:** To enhance the visual appeal of graphs.
- **NumPy and Pandas:** For numerical computations and data handling.

## Installation and Usage

### Requirements
- Python 3.x
- Required libraries:
  ```bash
  pip install mesa==2.3.3 matplotlib seaborn numpy pandas
  ```

### Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/carlosagalicia/Cleaning-Simulation.git
   ```

2. Navigate to the project directory and run the script:
   ```bash
   jupyter notebook cleaning_vacuums_simulation.ipynb
   ```

3. The program will execute the cleaning simulation and display the results, including animation and performance metrics.

## Visualization and Results
- The grid is visualized using Matplotlib to track the progress of cleaning over time.
- An animation of the cleaning process is created to observe agent behavior step by step.

## Example Output
- **Simulation Metrics:**
  - Total steps: `X` (varies based on parameters)
  - Efficiency per vacuum cleaner: Displayed in the terminal.
- **Visualization:**
  - Animated cleaning process of the grid.

## Customization Options
- Modify these parameters in the script to test different scenarios:
  - Room dimensions (`WIDTH`, `HEIGHT`)
  - Percentage of initial dirt (`DIRTY_CELLS`)
  - Number of vacuum agents (`VACUUMS`)

## Key Learning Areas

### 1. Agent-Based Modeling
- Designing agents with unique behaviors (Vacuum Cleaners and Dirt).
- Implementing interactions between agents and their environment.

### 2. Performance Evaluation
- Measuring and analyzing cleaning efficiency.
- Visualizing the agent-based simulation process.

### 3. Data Collection and Analysis
- Utilizing Mesa's `DataCollector` to record metrics at each simulation step.

## Visual Representation

### Cleaning Progress Animation
- The grid is animated to display the cleaning process, showing vacuums moving and cleaning dirt in real time.

## Visual Representation
<table>
<tr>
  <td width="50%">
    <h3 align="center">Dirty room with robots (initial state)</h3>
    <div align="center">
      <img src="https://github.com/user-attachments/assets/5391c299-0766-478d-9901-ded99ac27f6d">
    </div>
  </td>
</tr>
</table>

<table>
<tr>
  <td width="50%">
    <h3 align="center">Cleaned room (final state)</h3>
    <div align="center">
      <img src="https://github.com/user-attachments/assets/54177fdd-078a-455e-846d-bd4000bff325">
    </div>
  </td>
</tr>
</table>
