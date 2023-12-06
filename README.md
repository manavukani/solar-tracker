# solar-tracker
Solar Tracking for Optimization of Photovoltaic Power Generation

## Motivation
I am thrilled to share that Smart Cities are no longer just a theoretical concept, but a tangible reality in today's world. With the rapid pace of urbanization and industrialization, the demand for energy has never been higher. However, there is a silver lining - renewable energy is gaining immense popularity and can help us achieve sustainability. By leveraging IoT and data analytics, we can collect real-time data and build a robust system to optimize energy harvest from solar sources. This is an exciting time for us to come together and make a positive impact on our environment.

## Scope of Project
To achieve the maximum possible power output from a solar panel, it is necessary to enable it to track the sun and rotate and position itself accordingly. This will ensure that no part of the solar array is covered by shade due to any obstructing factors. To further optimize the power output, a smart mechanical system can be implemented to adjust the panel to a better angle and position, thereby re-obtaining maximum current and voltage.

## Methodology
An integrated system consisting of an Arduino Uno and a Raspberry Pi is used to collect and process data. Light Dependent Resistor (LDR) readings are taken from each corner of the solar panel, and the average values of all four sides are calculated. The panel is then adjusted to equalize the averages. Once a stable position is reached and a certain number of values are obtained, a simple linear regression model is trained. This model allows the panel to continue optimizing its positioning to obtain maximum sunlight. If the power being generated drops below regular levels, the sensors start sensing again, and the data collected is used to retrain the model for reconfiguration purposes.

## Results
A linear regressor model has been developed to adjust the positioning of a panel in order to obtain the maximum possible power over a period of time. The reconfiguring functionality has been successfully implemented, allowing the panel to adapt to changing trends and optimize the interfaced photovoltaic power generation. The system has been built successfully.

## Diagram
![image](https://github.com/manavukani/solar-tracker/assets/84531789/270702fc-9215-4257-8a78-7f8b9670e73f)
