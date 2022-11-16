## Homework: routing

_Vehicle routing_ is a geralization of the _Traveling Salesman Problem_. There are $N$ cities. Their pairwise distances are given by a matrix $Distance$. (You may assume that the matrix is symmetric.) We have $K$ vehicles. Each vehicle has a depot in one of the cities $1..N$. The depots are given by a list $Depot$. 

The goal is to plan routes for each vehicle so that each city is visited __at least once__ and each vehicle returns to its original depot. We want to minimize total distance traveled by the vehicles. (You can assume that the depot vehicles are already visited. The route of a vehicle may be empty, if it happens to be optimal.)

```
picat routing.pi instance.pi
```
Should return the optimal value of `??` and some representation of the route of each vehicle.
