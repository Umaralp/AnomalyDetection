# Python SIEM System Using AI and LLMs for Log Analysis and Anomaly Detection

## Overview
This project implements a Python-based SIEM (Security Information and Event Management) system that leverages AI and LLMs (Large Language Models) for log analysis and anomaly detection. The script `anomaly_demo_py.py` processes system logs, extracts relevant data, and identifies anomalies using statistical methods.

## Features
- Reads and parses system logs from text or CSV files.
- Converts logs into a structured pandas DataFrame for analysis.
- Simulates login attempts to generate normal and anomalous behavior.
- Detects anomalies in login attempts using statistical methods.
- Visualizes login attempts over time with highlighted anomalies.

## Installation
### Prerequisites
Ensure you have the following dependencies installed:
- Python 3.x (recommended python 3.6+)
- pandas
- numpy
- matplotlib

To install missing dependencies, run:
```bash
pip install pandas numpy matplotlib
```

## Usage
1. Clone the repository or download `anomaly_demo_py.py`.
2. Run the script in a Python environment:
   ```bash
   python anomaly_demo_py.py
   ```
3. The script will process log data, detect anomalies, and generate a visualization.

## Output
The script outputs:
- Parsed log data in a structured format.
- Identified anomalies in login attempts.
- A graph showing login attempts over time with anomalies marked in red.

![output](Screenshot%202025-03-09%20065543.png)

#### Console Output:
```
   timestamp              level  user   
0  2025-03-06 08:00:00   INFO   admin  
1  2025-03-06 08:01:23   INFO   alice  
2  2025-03-06 08:02:45   ERROR  alice  
Login attempts per minute: [ 5  4  3  5 ... 40 50 ]
Anomaly indices: [50 51 52]
Anomaly values (login attempts): [30 40 50]
```
![console output](Screenshot%202025-03-09%200620.png)
#### Graphical Output:
![anomaly detection Graph](Screenshot%2025-03-09%065630.png)

## Future Enhancements
- Integration with machine learning models for anomaly detection.
- Real-time log monitoring and alerting.
- Use of LLMs for advanced log analysis.

## License
This project is licensed under the MIT License.

## Author
Junaid Umar

