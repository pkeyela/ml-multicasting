This is one of the final versions of my Master's degree problem:

## Problem:
A base station is delivering through multicasting technique a particular service to N users (or user equipement) uniformly distributed in an area of radius $R$. Using a separate channel for every user is ressource waisting. It would be better to serve users "near" to another with a single beam. But the antennas can form only a fixed number of beams differing by their angle and the maximal radius they can reach. The Power and the BS is also a limited ressource. The goal is to find the most efficient way of forming the groups to be served by a single beam in the way that all the users are served and at minimal cost. The cost here is the number of ressource blocks used by BS to deliver the service unto the users.

The formulas in the notebook are the results of the analytical resolution (I designed an analytical algorithm to solve this optimization problem, taking into account the constrainst of limited power, SINR quality, the types of beams, the positions of the users)

The downside of my analytical solution is that it become slow with the growth of $N$ (it has exponential complexity). So I proposed to use ML algorithms which learn from the solutions on small $N$ to extrapolate on bigger number of user. 

I got results for 12, 15, 30 and 60 users but work is still to be done to build better models instead of using classical and simple algorithms.
