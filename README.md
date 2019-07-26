# slm
Mac version java wrapper for smart local moving (SLM) algorithm is an algorithm for community detection (or clustering) in large networks, modified based on Windows version of chen198328/slm


#  Change
change from as_data_frame() to igraph::as_data_frame() from master chen198328/slm ;
added parameter version= "Win" or "Mac"

# usage

the package is based on the jar file, so the system require java 1.8+ 

```r
devtools::install_github("chen198328/slm")

library(igraph)
library(igraphdata)
library(slm)

data("karate")

slm.cluster <-SLM.community(karate)
plot(slm.cluster, karate)
```

# plot
![image from host](http://ludowaltman.nl/slm/network.png)
