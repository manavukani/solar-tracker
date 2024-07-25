# Solar Tracking for Optimization of Photovoltaic Power Generation in Solar Panel

This project aims to optimize photovoltaic power generation using solar tracking technology. By leveraging IoT and data analytics, the system ensures that solar panels track the sun's position and adjust accordingly to maximize power output.

## Scope of Project

- **Need**: With the rapid pace of urbanization and industrialization, energy demand has surged. Renewable energy, particularly solar energy, offers a sustainable solution. By utilizing IoT and data analytics, we can build a system that optimizes solar energy harvest, contributing to smart city development and environmental sustainability.
- **Objective**: To achieve maximum possible power output from solar panels by tracking the sun and adjusting the panel's position to avoid shading and optimize the angle.
- **Implementation**: A smart mechanical system adjusts the panel to maintain optimal current and voltage, thereby maximizing power output.

## Outcome
![image](https://github.com/user-attachments/assets/a394d831-fecd-4413-b0ca-20c6ff2db1a4)


## Methodology

1. **System Integration**: 
    - An Arduino Uno and a Raspberry Pi are used to collect and process data.
    - Light Dependent Resistor (LDR) readings are taken from each corner of the solar panel.
    - Average values from the LDRs are calculated, and the panel adjusts to equalize these averages.

![image](https://github.com/manavukani/solar-tracker/assets/84531789/270702fc-9215-4257-8a78-7f8b9670e73f)
  
2. **Data Processing**:
    - A linear regression model is trained using the collected data to optimize the panel's positioning.
    - The model adjusts the panel for maximum sunlight based on real-time data.
    - If power generation drops below expected levels, sensors recalibrate and retrain the model.

3. **Results**:
    - A linear regressor model successfully adjusts the panel positioning for optimal power output.
    - The reconfiguration functionality adapts to changing conditions, optimizing photovoltaic power generation.

## Implementation Details

- **Hardware**:
  - Solar Panels
  - Light Dependent Resistors (LDRs)
  - Arduino Uno
  - Raspberry Pi
  - Servo Motors

- **Software**:
  - Python (for data processing and model training)
  - Arduino IDE (for interfacing with hardware)
  - Sklearn (for linear regression)

## Usage

1. **Setup**:
   - Connect the solar panel to the Arduino and Raspberry Pi.
   - Place LDRs at the corners of the solar panel.

2. **Running the System**:
   - Use the `sending.py` script to collect and process sensor data.
   - The `work.py` script trains the regression model and adjusts the panel positioning.

## Files

- `sending.py`: Collects data from the Arduino and stores it for model training.
- `work.py`: Trains the regression model and adjusts the panel positioning.

