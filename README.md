# IMS24052-DSC212

Discussion – Central Nodes and the Influence of Community Structure
1. Persistent central nodes

Degree centrality (within community):
Nodes that consistently appear among the top-ranked have many neighbors inside their community at each stage of splitting. In the Karate graph, well-known hub nodes (such as node 0, node 33, and others depending on the split sequence) typically remain central.

Betweenness centrality (within community):
Nodes that function as local bridges within a community tend to maintain higher betweenness values. Since betweenness depends on how connected a community is, its value changes noticeably if the community breaks into smaller parts.

Closeness centrality (within community):
Nodes positioned near the “center” of their community show high closeness because average path lengths become shorter in smaller subgraphs. Splits often increase closeness values in compact communities.

Clustering coefficient:
Nodes that lie in tightly connected triangular structures preserve high clustering. This measure often increases as communities split, because dense subgroups or cliques become isolated.

2. How community structure affects metrics

Local instead of global influence:
Recursive splitting separates closely connected groups, so centrality values calculated on subgraphs reflect local cohesion rather than global importance. A node that was globally central may no longer dominate once some of its connections fall into other communities.

Betweenness is highly sensitive to splits:
Nodes that originally acted as bridges between major parts of the graph lose betweenness once those regions are placed in different communities.

Closeness rises in smaller communities:
As community size decreases, average distances shrink. However, the ranking of nodes can still shift if some of their neighbors are moved to other groups.

Clustering tends to increase:
Community splits frequently isolate small, dense clusters, causing higher local clustering values.

3. Practical takeaway

Hierarchical structure becomes visible:
Recursive spectral modularity reveals structure at multiple levels—early splits show broad divisions (e.g., leader-based factions), while later splits highlight fine-grained local groups.

Community-based centrality gives local influence insights:
Measuring centrality inside each node’s current community highlights nodes that are important for local cohesion or information spread, rather than those that are globally influential.
