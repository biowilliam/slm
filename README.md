# slm
This repository is Mac/Windows R wrapper version of smart local moving (SLM) algorithm initially implemented in Java.  

The SLM algorithm maximizes a so-called modularity function. The algorithm has been successfully applied to networks with tens of millions of nodes and hundreds of millions of edges. The details of the algorithm are documented in a paper (Waltman & Van Eck, 2013).  
The SLM algorithm has been implemented in the Modularity Optimizer, a simple command-line computer program written in Java. The Modularity Optimizer can be freely downloaded (http://www.ludowaltman.nl/slm/) (last updated: August 31, 2015). The program can be run on any system with Java support. In addition to the SLM algorithm, the Modularity Optimizer also provides an implementation of the well-known Louvain algorithm for large-scale community detection developed by Blondel, Guillaume, Lambiotte, and Lefebvre (2008). An extension of the Louvain algorithm with a multilevel refinement procedure, as proposed by Rotta and Noack (2011), is implemented as well. All algorithms implemented in the Modularity Optimizer support the use of a resolution parameter to determine the granularity level at which communities are detected.




# Usage

the package is based on the jar file, so the system require java 1.8+ 

# Updates
Waltman & Van Eck recommend their latested Leiden algorithm 2018 instead (https://github.com/CWTSLeiden/networkanalysis#compilation).


```r
devtools::install_github("biowilliam/slm")

library(igraph)
library(igraphdata)
library(slm)

data("karate")

slm.cluster <-SLM.community(karate)
plot(slm.cluster, karate)
```

# plot
![image from host](http://ludowaltman.nl/slm/network.png)
