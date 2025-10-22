#### Problem Description:

Drone Delivery Problem is a Stochastic Multi-hospital Allocation and Recharging for Transportation (SMART) problem, which considers a network of 𝐻 medical facilities, each receiving a stochastic number of requests for medical items over time, modeled by a known distribution. A fleet of 𝑀 drones, each with varying state-of-charge (soc), each with distinct load capacities,  operates from a hub equipped with both slow and fast chargers and stocked with medical supplies. The system is looking for a balance between efficiency and cost while meeting varying demand. Optimal operational decisions in this dynamic setting involve determining whether a drone should be dispatched to satisfy a hospital’s demand (which drone to which hospital), recharged using fast or slow chargers in anticipation of future tasks, or kept idle to conserve resources. The objective is to maximize the expected total reward, defined as the weighted sum of satisfied demand across all hospitals and time periods. Although the primary focus of the system is to meet as much demand as possible, we put penalties in the objective function for using slow and fast chargers to account for different degradation rates and charging costs.We proceed by describing the important assumptions considered in this paper before presenting the problem formulation.





#### Assumptions:

* Stochastic demand for each hospital follows a non-homogeneous Poisson distribution.
* A safety-reserve battery’s soc is enforced to keep a minimum power inside the batteries after missions.
* Given the time-sensitive nature of delivering medical items, backlogging unmet demand is not allowed.
* We approximate the required time and gained energy during charging batteries with a three-threshold piecewise-linear function.
* We assume a constant charge decrement over the flight time.
* The hub has sufficient fast and slow chargers to accommodate all drones without resource bottlenecks.
