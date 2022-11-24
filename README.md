## Homework: routing

_Vehicle routing_ is a geralization of the _Traveling Salesman Problem_. There are $N$ cities. Their pairwise (integer) distances are given by a matrix $Distance$. (You may assume that the matrix is symmetric, with 0s on the main diagonal.) We have $K$ vehicles. Each vehicle has a depot in one of the cities $1..N$. The depots are given by a list $Depot$. 

The goal is to plan routes for each vehicle so that each city is visited at least once and each vehicle returns to its original depot. We want to minimize total distance traveled by the vehicles. (You can assume that the depot cities are already visited. The route of a vehicle may be empty, if it happens to be optimal.)

Use the constraint `subcircuit` in your model. Running

```
picat routing.pi instance.pi
```
should return the optimal value of `34` and some representation of the route of each vehicle.

