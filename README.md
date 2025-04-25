# Truck-Drone-Delivery-System!!!

An innovative solution for last-mile delivery of packages is to use a truck and drone combination package delivery system wherein a truck operates with a fleet of drones to deliver packages. The truck travels to a customer location which can be used as a launch site for the drones to reach other customers that are in vicinity of the visited customer. This gives rise to a new variant of the Travelling Salesman Problem (TSP) called the Flying Sidekick Travelling Salesman Problem (FSTSP). In TSP, we make sure that each customer is visited exactly once by the truck. In FSTSP, we make sure that each customer is visited exactly once by either the truck or the drone. 

In this I have formulated the truck-drone combination package delivery system as a mixed integer programming problem with the objective of minimizing cost subject to following constraints and solving it using Xpress-MP - 

Constraints:
- The truck must start and end at the depot.
- The truck can deploy up to K drones at each stop in a launch site.
- The drones have limited cargo capacity and as a result they can only visit 1 customer (not counting the starting point) before returning to the truck.
- Each customer should be visited at least once by a drone. The customer locations used as launch sites will be visited by the truck and also will serve as the starting and ending point of a drone tour.

Assumptions
- Assume that the depot is located at the origin (0,0).
- For each unit of distance traveled by the truck there is a cost of $10, while for each unit of distance traveled by a drone there is a cost of $3.