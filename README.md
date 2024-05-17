# PulseMaster

PulseMaster is an electrical pacmaker engineered to synchronize, sense, and deliver precise electrical impulses to the heart as necessary. These electrical signals, transmitted through strategically placed 
electrodes, allow for the contractions of the heart chambers, ensuring an optimal blood-pumping rhythm. 

## Interface

PulseMaster is provided with a cutting-edge interface designed in Python that allows the doctor to customize each electrical pacemaker for each unique patient, and observe real time data of the pacemaker working in different scenarios.
- 8 possible modes to configure from: VOO, VVI, AOO, AAI, AOOR, AAIR, VOOR, VVIR
- Over 20 different parameters to configure for each mode, such as LRL, URL, VA, VPW, etc
- Up to 10 accounts can be made for different patients, with user authentication
- Interface knows when the pacemaker is connected to the device the interface is on, and can flash the new settings onto the pacemaker
- Interface allows the pacemaker to start running once values are flashed, and will not start any other way for safety precautions.
- Real time graphs are given to visualize the atrial and ventricular modes, in terms of time and voltage provided

## Functionality

The functionality of the pacemaker is designed in Simulink, providing quick response times and decision making. This allows for the pacemaker to detect when the heart needs assistance and if it always needs assistance, and provide the
correct amount of voltage at the correct time to simulate a heart beat.
- Can detect when a heartbeat is needed from the electrical pacemaker
- Can produce a heartbeat at the correct voltage/time
- Can detect which activity the user is in, from sitting, to walking, to running
- Can produce different paces/voltages based on the mode provided by the interface
