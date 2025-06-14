# Predictive-Analysis-for-BLEVE
 predictive analysis on the peak pressure generated by Boiling Liquid Expanding Vapour Explosions (BLEVEs).
![image](https://github.com/user-attachments/assets/8536fc0c-9a4e-49a2-99b2-158ea149f6d0)
![image](https://github.com/user-attachments/assets/7e7c9b37-0e80-451e-b221-ea87624ec4d0)

Libraries: pySpark, pandas, scikit-learn, tensorflow

Consider a scenario where a BLEVE occurs inside a rectangular tank located within a three-dimensional environment, as
illustrated in Figure 1. A rigid wall, simulating a building structure, is placed at a certain
distance from the BLEVE source. This wall interacts with the blast wave, causing reflections
and deflections that increase the complexity of the pressure distribution.
The objective is to accurately predict the peak pressure in the vicinity of the obstacle. To
support this task, 27 sensors are strategically placed around the obstacle walls—nine each
on the front, back, and side walls—as shown in Figure 2. These sensors are used both for
training and testing the predictive model.
The 3D environment includes a variety of physical variables relevant to BLEVE scenarios,
such as temperature, pressure, gas-to-liquid ratio, and the dimensions of both the tank and
the obstacle. The full list of input features is as follows:
• Tank Failure Pressure: internal pressure at the time of BLEVE (in bar)

• Liquid Ratio: ratio of liquid in the tank (coexistence of liquid and vapour)

• Tank Width: tank width (in metres)

• Tank Length: tank length (in metres)

• Tank Height: tank height (in metres)

• Vapour Height: vapour column height inside the tank (in metres)

• BLEVE Height: height of the tank above ground level (in metres)

• Vapour Temperature: temperature of vapour (in K)

• Liquid Temperature: temperature of liquid (in K)

• Obstacle Distance to BLEVE: distance between the obstacle and BLEVE source (in metres)

• Obstacle Width: obstacle width (in metres)

• Obstacle Height: obstacle height (in metres)

• Obstacle Thickness: obstacle thickness (in metres)

• Obstacle Angle: angle between the line connecting the centres of the obstacle and BLEVE and the horizontal axis (in degrees)

• Status: liquid state, either subcooled or superheated

• Substance Critical Pressure: pressure required to liquefy vapour at the critical temperature (in bar)

• Substance Boiling Temperature: boiling point at atmospheric pressure (in C)

• Substance Critical Temperature: temperature above which vapour cannot be liquefied regardless of pressure (in C)

• Sensor ID: unique identifier of the sensor (ranging from 1 to 27)

• Sensor Position Side: side of the obstacle where the sensor is located

• Sensor Position x: x-coordinate of the sensor (in metres)

• Sensor Position y: y-coordinate of the sensor (in metres)

• Sensor Position z: z-coordinate of the sensor (in metres)

• Target Pressure: peak pressure to be predicted (in bar)
