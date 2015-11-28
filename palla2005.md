# Uncovering the overlapping community structure of complex networks in nature and society
*Palla, Derenyi, Farkas, Vicsek*

* The existing deterministic methods used for large networks find separated communities, whereas most of the actual networks are made of highly overlapping cohesive groups of nodes.
* overlaps are significant, and the distributions we introduce reveal universal features of networks
* web of communities has non-trivial correlations and specific scaling properties

## Definition community
* parts in which the nodes (units) are more highly connected to each other than to the rest of the network (are called: clusters, communities, cohesive groups, modules)
* most real networks are characterized by well-defined statistics of overlapping and nested communities
* has never been studies for large networks

## Basic quantities
* node `i`
* **membership number** `m_i` ... number of communities the node `i` belongs to
* any two communities `A` and `B` can share `s_ov` nodes ... **overlap size** between these communities
* communities constitute a network (each community is a node, links are overlaps)
* **community degree** of a community is called `d` ... number of such links
* **size of community** `s_com` is defined as number of its nodes
* to characterize community structure of network we introduce the distribution of these four basic quantities

## Cummulative distribution functions
* `P(m)` ... number of communities a node belongs to (membership number)
* `P(s_ov)` ... number of nodes two communities share (overlap size)
* `P(d_com)` ... degree of a community-node (communiy degree)
* `P(s_com)` ... size of community (communiy size)
* `P(s_ov)` means  the proportion of thos overlaps that are larger than `s_ov`

## Formal definition of community
* a typical community consists of several complete (fully connected) subgraphs that tend to share many of their nodes
* **`k`-clique community:** union of all `k`-cliques (complete subgraph of size `k`) that can be reached from each other through a series of adjacent `k`-cliques (where adjacency means sharing `k-1` nodes)
* Basic requirement:
** it cannot be too restrictive
** should be based on density of links
** required to be local
** should not contain any cut-link or cut-node
** should allow overlaps

## Methods for finding communities
* clique percolation
* divisive method (cut network in smaller and smaller pices)
* agglomerative method (do same as divisive but reverse order)

## `k` and `w*`
* `k` size of clique and `w*` is a treshhold for edge weights
* goal is to find a giant component
* for each `k={3,4,5,6}` the treshhold `w*` is lowered until the largest community becomes twice as big as the second largest one
* `f*` is fraction of links stronger than `w*`
* choose only values for `k` for which `f*` is not too small (not smaller than 0.5)
* -> `k = 6 | 5` with `f* = 0.93 | 0.75` for collaboration networks

## Analyzing distribution of the 4 properties
* **Community size** follows a power law
* **Community degree** not following power law: exponential + power law tail
* **Overlap size** follows power law
* **Membership Number** close to powr law
