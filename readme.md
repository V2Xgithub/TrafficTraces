# Trace File
There are two kinds of files here:
1. traffic trace file
2. obstacles map file
## Data format
### 1. traffic trace file
|Time [s]|Vehicle ID|X-axis coordinate [m]|Y-axis coordinate [m]|Speed [m/s] (if have)|
|:---:|:---:|:---:|:---:|:---:|
|0|1|8523|8081|
|0|2|8554|8155|
|0|3|8611|8449|
|0|4|8635|8453|
|....|
|19|48|9684|9095|
|20|291|8593|8709|

### 2. obstacles map file
This file is for LOS/NLOS evaluations. If you open this .txt file, you could see the map. And people could adjust the map easily.
* line 1: XminMap, XmaxMap, YminMap, YmaxMap, StepMap(or granularity)
* line 2~end: composed of [0, 1], stands for the building (0) or street (1)