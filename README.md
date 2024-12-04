# CV_project1

## Project Goal
Develop an algorithm to detect and track moving objects in acoustic data collected from a Distributed Acoustic Sensing (DAS) system attached to the fiber optic cable at Jana Pawla II Street.

(Standard version 4)
Your task is to load the data, filter out the noise and process it in such a way that only moving objects (slanted lines) are visible. Then You need to determine the velocity for these objects (see the figure on the next page).

(Version for 5):
Instead of a single value of the object's speed, draw a graph of the speed changing over time.
Add clustering of objects into several groups differing in the nature of the signal, e.g. thick line, narrow line, objects with constant speed, objects with changing speed.

Distributed Acoustic Sensing (DAS) is an advanced technology that transforms optical fiber cables into highly sensitive vibration sensors. By sending pulses of laser light through a fiber optic cable and analyzing the backscattered light, DAS systems can detect subtle strain variations along the fiber, which may be caused by seismic activity, traffic, or small object movements. These variations are recorded as phase shifts in the backscattered light signal, which correlate directly to the fiber's strain. With appropriate calibration, these phase shifts are processed to measure strain or strain rate over time. The resulting time-series data provides a detailed, chronological record of vibrations along the fiber, allowing for further analysis to identify the source, magnitude, and frequency of disturbances.


## Input Data
The data is stored in numpy format as a 2D matrix. The particular value represents the strain rate of a fiber optic cable located on a busy street (Jana Pawla II). The data shows the passage of trams, trucks or cars along this street.
The first dimension is time, the second is space, in order to calculate the correct units use the following metadata:

* dx: 5.106500953873407 [m]
* dt: 0.0016 [s]
* file duration: 10s
* number of time samples in file: 6250
* file name format: HHMMSS
* files date: 2024-05-07

## Requirements
* The implementation of the algorithm must be created in Python with use the following image processing libraries: OpenCV, NumPy, Matplotlib, Pillow, and Skimage. If You want to use other libraries, consult by e-mail (do not use neural networks or external tools).
* The solution must contain the source code and a report describing the algorithm along with a description of intermediate steps and the experiments performed (if you have tested several successful/unsuccessful solutions, describe them)
* The solution can be presented in the form of source code (.py) and an attached report (.pdf) or a jupyter notebook file ( .ipynyb and one of .pdf or .html) containing the code and description of the next steps
* Images in the report can be scaled down so that the report is not too large.
* All sources of data, code and inspiration must be reported with a description of what was used.

The project can be done in pairs.

Deadline for sending the code, and report: 4.12.2024 23:59

The project will be presented in class 4.12.2024
