# Microsoft Open Source Hackthon 2020


***TEAM: TECHNO PANDITS***

**Problem Statement**

*Smart Traffic Management System for Quick Commute and Carbon Reduction*

Traffic congestion is rising in cities around the world. Contributing factors include expanding urban population, aging infrastructure, inefficient and uncoordinated traffic signal timing and a lack of real-time data.

Advanced traffic management technologies such as adaptive traffic control and traffic analytics can improve safety and significantly decrease traffic congestion levels and greenhouse gas (GHG) emissions.

Create a solution for smart cities with mature traffic management.





**Idea**

We are aiming to solve the traffic congestion problem by optimising the signal timer durations. This will be done by setting the timers proportional to their respective road traffic density. 
Do take a look at the Presentation Created by Us: CodeForTheFuture_TechnoPandits.pdf




**Approach**
* The first step is to find traffic flow on every side of a crossroad. This is done by fetching data from 'Traffic Flow' API. Here we have used [Azure Maps API](https://azure.microsoft.com/en-in/services/azure-maps/).  Azure Maps API is one of the leading traffic flow API with an accuracy over 96%. This traffic density data will be used in real-time to calculate the wait time for each signal.
* Now that our model has the traffic distribution along the crossroad, the next step would be to find optimal trffic signal timings. We try to optimize signal timings by focusing more on **_equity_ over equality.** In simple words, the signal wait time would be indirectly proportional to the traffic flow on a side rather than having same wait time for all sides of the crossroad.
So, for eg on a 4-way crossroad, if one of the roads has a greater traffic density, then, the signal wait time will be proportionally lower.
* After finding optimal signal timings, the signal timers are set as per those timings.
* The whole process is repeated after an interval of 2 min. This is done to achieve the **real time** aspect of our model.

## Flowchart of Model :-
![Flowchart](https://github.com/sanky2501/Microsoft-Hackthon/blob/master/Flowchart.jpg)

## Structure of Model
![Structure](https://github.com/sanky2501/Microsoft-Hackthon/blob/master/Structure.PNG)


**devDependencies**
* [Jupyter Notebook](https://jupyter.org/)(Python version 3.7.2)
* [Azure Maps API](https://azure.microsoft.com/en-in/services/azure-maps/)


**Python Libraries Used**
* numpy
* random
* time
* json
* requests

**REPO:**

**STEP 1:** Calculate the Traffic Signal Timer formula for a Cross-Road. (Sample Data used instead of Real Time Data)

**FILE:**  [Signal Timer Model 1](Signal_Timer_Model_1.ipynb)


**STEP 2:** Accessing Real Time Data. (Trial was Done Using TomTom API - Later Shifted to AZURE MAPS API)

**FILE:** [Signal Timer Model 2](https://github.com/sanky2501/Microsoft-Hackthon/blob/master/Signal%20Timer%20Model%202.ipynb)


**STEP 3:** Integration of STEP 1 and STEP 2 - Using Real Time data with Signal Timer Algorithm

**FILES:** [Integration 1](https://github.com/sanky2501/Microsoft-Hackthon/blob/master/Integration%201.ipynb), [Integration 2](https://github.com/sanky2501/Microsoft-Hackthon/blob/master/Integration%202.ipynb)

We have implemented our model on a crossroad in Pune called as [Parihar Chowk](https://www.google.com/maps/place/Parihar+Chowk,+Sanghvi+Nagar,+Ward+No.+8,+Aundh+Gaon,+Aundh,+Pune,+Maharashtra+411007/@18.5608719,73.8079131,17z/data=!4m5!3m4!1s0x3bc2bf307ea957bd:0x981c13e6518c2913!8m2!3d18.5606075!4d73.8092435).

Following are the locations of each side that are fed to Azure Maps API to fetch traffic flow on each side.
[Side1](https://github.com/sanky2501/Microsoft-Hackthon/blob/master/parihar1.PNG), [Side 2](https://github.com/sanky2501/Microsoft-Hackthon/blob/master/parihar2.PNG), [Side 3](https://github.com/sanky2501/Microsoft-Hackthon/blob/master/parihar3.PNG), [Side 4](https://github.com/sanky2501/Microsoft-Hackthon/blob/master/parihar4.PNG)

To better understand about the locations fed to API refer the diagram below :-
* A RED Dot denotes a location fed to the API

![API Locations](https://github.com/sanky2501/Microsoft-Hackthon/blob/master/72dadc01-1964-448e-8b3f-1141eb0debac.jpg)

## Advantages of our Model :-
* Real-Time Solution
* Addresses All Ranges of Traffic Densities
* Low Maintenance Cost  
* High Accuracy and Consistency
* Does Not Depend on any External Factors like Weather, Road Construction, Human Intervention, etc

## Drawback :-
* The model may not work efficiently if the locations fed to the Maps API are not precise. 

## Future Scope:-
* Include Pedestrian Timers
* Integrating with other traffic solutions

**Integration 2.ipynb is our _FINAL PROTOTYPE._**

The project has also been uploaded on [Azure Repo](https://notebooks.azure.com/sgumredkar/projects/microsoft-code-for-future).

