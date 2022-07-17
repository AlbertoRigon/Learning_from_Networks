# Learning from Networks
This repository contains a project developed together with [Luca Scattolaro](https://github.com/LucaScattolaro) and [Alessandro Chimetto](https://github.com/ChimeBello) for the Learning from Networks 2021/2022 course attended at Università degli Studi di Padova. The goals of this project are:
- Find the most influent people on **Twitch** by computing popular detailed measurements such as closeness centrality, betweenness centrality, and clustering coefficients for all nodes;
- Understand what motifs are more prevalent in order to discover and analyze the underlying structure of Twitch's network.

My main contribution is the `ApproximatedCentralitiesLibrary.py`. For this project, we used the [*Twitch Gamers Social Network*](https://snap.stanford.edu/data/twitch_gamers.html) dataset.

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


