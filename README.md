# Learning from Networks
This repository contains a project developed together with [Luca Scattolaro](https://github.com/LucaScattolaro) and [Alessandro Chimetto](https://github.com/ChimeBello) for the Learning from Networks 2021/2022 course attended at Università degli Studi di Padova. My main contribution is the `ApproximatedCentralitiesLibrary.py`.

### Graph Library
**Graph Library** is defined in `graphLibrary.py`. It contains all the methods to compute centralities, clustering coefficients and motifs plus some helper functions that allow to draw graphs, save the results in a `.csv` file or produce a ranking of scores (e.g. for the centralities). To import the library:
```
import graphLibrary as gl
```
Then, you can call the functions from code as:
```
closeness = gl.approximated_closeness_centrality(G, k)
betweenness = gl.approximated_betweenness_centrality(G, epsilon)
...
```

### Usage
A script `Project_LFN.py` that allows you to test all the methods is provided. Notice that these implementations are designed to work on `networkx` graphs. 


