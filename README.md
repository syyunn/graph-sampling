# graph-sampling
Lists up the graph sampling strategy to statistically learn the large scale graph

Following discernment mainly referred from
https://bmcbioinformatics.biomedcentral.com/track/pdf/10.1186/s12859-019-2914-2

## Homogeneous Only

### DeepWalk 
DeepWalk deploys a truncated random walk to sample node sequences, and uses the skip-gram model to learn the representation of node sequences
- only considers the first-order proximity between nodes.
- only applies to unweighted networks

### LINE
- LINE is applicable for both weighted and unweighted networks 
- easily scales to large-scale networks with millions of nodes. 
- The problem is that embedding of some loosely-connected nodes, which have few connected edges, heavily depends on their connected neighbors and unconnected negative samples

### Node2Vec

## Heterogeneous 
### metapath2vec
