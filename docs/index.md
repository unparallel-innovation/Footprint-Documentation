# Footprint

FOOTPRINT is an edge device that enables a high-level monitoring of the production quality, automatic detection and identification of problems or defects during manufacturing. The edge device uses voltage and current sensors to provides energy monitoring and detection of the machine’s job or action based on the energy profiles used to train the model. Additionally, automatic detection and identification of problems or defects during manufacturing and maintenance forecasts can also be supported.

The FOOTPRINT edge device has 4 inputs for current measurement (L1, L2, L3, N) and three inputs for voltage measurement. This allows measurements on all three phases and the neutral conductor. The system is supplied with the required operating voltage via the L1 voltage connection, thus a separate power supply is not required. All interfaces to the system are galvanically isolated to ensure maximum safety. The housing has a mounting bracket on the back for mounting the system on a DIN rail, allowing easy installation.

##### Measured parameters:
- Current
- Voltage
- Power
    - Active power
    - Reactive power
    - Apparent power
- Energy consumption
- Energy production
- Power consumption
- Power production
- Frequency
- Power Factor

The measured parameters are read out every second and sent to the configured MQTT broker, for persistent storage of historical data in an external database. The data is also stored in an internal database every minute, which is convenient in case of offline usage. The measurement periods can be configured if needed, to match the requirements of the specific application scenario.

A dashboard, built with Grafana, is provided to view real time and historical data. The dashboard also supports exporting the historical data as CSV files, to allow usage of the datasets with other tools. Furthermore, with the integrated RESTful service, it is possible read out all relevant values directly out of the edge device.
