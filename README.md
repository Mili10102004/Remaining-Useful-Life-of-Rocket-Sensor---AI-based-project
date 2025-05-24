Predictive Maintenance for 
Reusable Rocket 
Components 
Prepared By 
Vraj Vyas (22000884) 
Vedant Gandhi (22000788) 
Om Pandit (22000658) 
Vaidik Patel (22000842) 
Mili Patel (2000902) 
1 
2 
 
 
 
 Table of Contents  
Problem Statement ....................................................................................... 3 
Dataset .......................................................................................................... 4 
Methodology ................................................................................................. 6 
Code: ........................................................................................................ 8 
Results ........................................................................................................ 16 
Challenges .................................................................................................. 21 
 
 
 
  
Problem Statement 
The core objective of this project is to enable predictive 
maintenance for reusable rocket components by accurately 
forecasting the Remaining Useful Life (RUL) of each component. 
In aerospace systems, especially reusable rocket engines, timely 
maintenance decisions are critical for ensuring safety, performance, 
and cost- efficiency. Predicting how many operational cycles remain 
before a component fails can significantly improve planning and 
reliability, 
thereby reducing downtime and unnecessary 
maintenance. 
This project aims to develop a machine learning model that can learn 
from historical sensor data and operational settings to predict the 
number of life cycles an engine or component can undergo before 
reaching a failure point. 
3 
Dataset 
The project utilizes multivariate time series data representing a fleet 
of engines operating under various conditions. The dataset is divided 
into training and test subsets for four different configurations: 
FD001, FD002, FD003, and FD004. Each time series corresponds 
to a different engine unit. 
Dataset Characteristics: 
 
 
 
Format: Space-separated text files (zip-compressed) 
Columns (26 total): 
o Unit number 
o Time (in cycles) 
o Operational setting 1–3 
o Sensor measurements 1–26 
Properties: 
o Sensor data contains noise. 
o Engines have unknown initial wear and manufacturing variance. 
o Time series for each engine starts with normal 
operation and gradually degrades. 
Data Subsets: 
 
FD001: 
o 100 train + 100 test trajectories 
o One operating condition (Sea Level) 
o One fault mode (HPC Degradation) 
4 
 
FD002: 
 
 
o 260 train + 259 test trajectories 
o Six operating conditions 
o One fault mode (HPC degradation) 
FD003: 
o 100 train + 100 test trajectories 
o One operating condition (Sea Level) 
o Two fault modes (HPC degradation, Fan degradation) 
FD004: 
o 248 train + 249 test trajectories 
o Six operating conditions 
o Two fault modes (HPC degradation, Fan degradation) 

