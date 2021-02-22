# ResilienceNet
# ResilienceNet
A package for network resilience assessment and planning with R. <br /> <br />
The overall aim is to provide reproducible and accessible tool to examine transit resilience at macro, meso and micro levels and thus inform transport policy and resilient planning. 

•	**At macro level**, the Package could not only produce ten key resileince related metrics but also simulate the planned and unplaned disruptions on transit networks through percolation approach. 

•	**At  meso level**, the Package helps planners better understand the roles of stations: the withinn-community contribution and inter-communiyt contribution.  

•	**At micro level**, the package mainly estimates how the disruption of station would affect passengers in terms of how many passengers cannot fulfil their travel and how much additonal travel cost (time and money) would cause. 

ResilienceNet should be useful to researchers interested in transport network and disruption modelling.


## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Key Functions
``` r
library(ResilienceNet)
macro.resilience (graph)
```
**At macro level, we can use rn_macro function to get a big picture of the general resilience performance of graph.**<br /><br />
Let's look at the macro resilience metrics:
<img width="944" alt="1" src="https://user-images.githubusercontent.com/51216959/108700398-721dc180-74fe-11eb-8473-188bea39da6d.png">


**At macro level, we can also include a dynamic perspective (percolation simulaiton) to look the resilience performance.**<br /><br />
``` r
g.gc_percolation(graph, cen=("deg", "bet", "clo"))

g.gc_percolation_random(graph)
```
![Image description](Images/Macro_percolation_sample.png)



### Installing

```
install.packages("devtools")
library(devtools)
install_github("YuerongZhang/ResilienceNet")
library(ResilienceNet)
```

## Built With

* [Igraph](https://github.com/igraph/igraph) is a C library for creating, manipulating and analysing graphs. 


## Versioning

0.1.0

## Authors

* **Yuerong Zhang** - *Initial work* - [Profile](https://www.ucl.ac.uk/bartlett/planning/yuerong-zhang)

See also the list of [contributors](https://github.com/xxxxx) who participated in this project.

## Acknowledgments

* Thanks to anyone whose code was used</pre>
