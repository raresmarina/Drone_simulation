# Drone_simulation
We have a drone, placed in a nunknown environment. We want this drone to map this environment into a predefined area.
In order to simplify the problem we consider only the movement in plan.
First step is to model this environment. The drone will explore a certain rectangular area A. We divide this area in small squares of size length u that will fit loosely thedrone(letssayu=55cm).If thesquare is emptyi twill be marked zero,if it is occupied it is marked with 1.
The problem modeled like this is reduced to map a simple labyrinth. For this we use 4 of the UltrasonicDistanceMeasuringSensors.The 4 sensors will give us the distances to the obstacles from a point in 4 directions.
So the drone’s sensor swil ldetect the 3u,0,u,and u values. So in order to map the surroundings we will need to move the drone,more or less, on each empty square at least one time. Consider now an algorithm like DFS, oro ther of the same type,and we want to map the surroundings with it.
