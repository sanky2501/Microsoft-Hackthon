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
The first step is to find traffic flow on every side of a crossroad. This is done by fetching data from 'Traffic Flow' API. Here we have used Azure Maps API
Traffic Density will be tracked using a ‘Traffic Flow’ API. This traffic density data will be used in real-time to calculate the wait time for each signal. So, for eg on a 4-way crossroad, if one of the roads has a greater traffic density, then, the signal wait time will be proportionally lower. 


**devDependencies**
* Jupyter Notebook
* Azure Maps API


**REPO:**

**STEP 1:** Calculate the Traffic Signal Timer formula for a Cross-Road. (Used Random Integer Instead of Real Time Data)

**FILE:**  [Signal_Timer_Model_1](Signal_Timer_Model_1.ipynb)


**STEP 2:** Accessing Real Time Data. (Trial was Done Using TomTom API - Later Shifted to AZURE MAPS API)

**FILE:** [Signal_Timer_Model_2](Signal_Timer_Model_2.ipynb)


**STEP 3:** Integration of STEP 1 and STEP 2 - Using Real Time data with Signal Timer Algorithm

**FILES:** Integration 1.ipynb, Integration 2.ipynb, parihar1.PNG, parihar2.PNG, parihar3.PNG, parihar4.PNG


**Integration 2.ipynb is our _PROTOTYPE._**

The project has also been uploaded on [Azure Repo](https://notebooks.azure.com/sgumredkar/projects/microsoft-code-for-future).

