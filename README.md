# Memristor Cycle Plotting Tool

A PyQt5-based GUI application for visualizing and analyzing memristor I-V characteristics from cycling data. Designed for researchers working with resistive switching devices, particularly halide perovskite memristors.

## Features

- **Interactive CSV Loading**: Import memristor cycling data with voltage and current measurements
- **Flexible Cycle Selection**: Choose specific cycle ranges or individual cycles to visualize
- **Set/Reset Sweep Filtering**: Toggle between set and reset operations for detailed analysis
- **Forward/Reverse Visualization**: Automatically distinguishes forward and reverse voltage sweeps with different line styles
- **Dual Axis Scaling**: Switch between linear and logarithmic current scales
- **Custom Axis Limits**: Manually set voltage and current ranges for focused analysis
- **High-Quality Export**: Save publication-ready figures in PNG, PDF, or SVG formats
- **Zoom and Pan**: Built-in matplotlib navigation toolbar for detailed inspection

## Installation

### Prerequisites

Ensure you have Python 3.7 or higher installed.

### Install Dependencies

```bash
pip install -r requirements.txt
```
## Usage
Running the Application
```bash
python set_reset_plotting_app_modified_v2.py
```
## CSV Data Format
Your CSV file should contain the following columns:
- *Cycle*: Cycle number (integer)
- *SetReset*: Operation type ("Set" or "Reset")
- *Voltage (V)*: Applied voltage in volts
- *Current (A)*: Measured current in amperes

## Workflow
Click Load CSV and select your data file
Use the Cycle Selection spinners to choose a range or manually select cycles from the list
Toggle Set and Reset checkboxes to filter sweep types
Choose Linear or Log scale for current visualization
(Optional) Set custom axis limits for focused views
Click Plot Selected Cycles to generate the visualization
Use the toolbar to zoom, pan, or reset the view
Click Save Figure to export your plot

## Output

The application displays I-V curves with:
Color-coded cycles for easy tracking
Solid lines for forward sweeps (positive to negative for Set, negative to positive for Reset)
Dashed lines for reverse sweeps
Current values automatically converted to milliamperes (mA)
Absolute values shown when using logarithmic scale

## Use Cases
This tool is particularly useful for:

- Characterizing memristor switching behavior
- Analyzing cycle-to-cycle variability in resistive switching devices
- Preparing figures for research publications
- High-throughput data visualization from electrical characterization

## The code is developed with the help of Claude Sonnet and ChatGPT by Rohit Attri
