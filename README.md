# slm
Mac version java wrapper for smart local moving (SLM) algorithm is an algorithm for community detection (or clustering) in large networks, modified based on Windows version of chen198328/slm


#  Change
change from as_data_frame() to igraph::as_data_frame() from master chen198328/slm
## windows version:
jar.path <- paste('"', jar.path, '"', sep = "") 
input.quote <- paste('"', input, '"', sep = "")
 output.quote <- paste('"', output, '"', sep = "")
## Mac version:
input.quote  <- input
output.quote <- output

# usage

the package is based on the jar file, so the system require java 1.8+ 

```r
devtools::install_github("chen198328/slm")

library(igraph)
library(igraphdata)
library(slm)

data("karate")

slm <-slm.community(karate)
plot(slm.karate)
```

# plot
![image from host](http://ludowaltman.nl/slm/network.png)
