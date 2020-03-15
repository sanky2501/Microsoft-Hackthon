# Microsoft-Hackthon
Microsoft Open Source Hackthon

Current Status:

We have created a small model similar to our idea. The final model will take input from API and the output will essentially be a timer. We are yet to add an API to our model (working on it currently).  
Do take a look at it and let us know what all changes we can make in the basic structure. 


We are trying to use ML to find:
1.	Busiest Hours and Idle Hours
2.	Balance between Efficiency and Fairness
e.g. – In the above proposed model, we have used 2 mins cycle time. In these 2 mins, each signal will be on at-least once. In this 2 min duration, our model ensures that it is fair in giving equal priority to all vehicles to cross the signal. But it does not ensure optimality, because if there is a heavy traffic density on the other side of the road, 2 mins is a short duration for that traffic to clear. We want to achieve perfect balance between fairness and optimality (which is essentially finding out the signal cycle time).
We want to achieve this balance with the help of an AI model which will be able to predict optimal yet fair tarffic signal durations.


Do let us know your suggestions on what all changes we can make to improve our solution and also guide us on implementing the AI model.
