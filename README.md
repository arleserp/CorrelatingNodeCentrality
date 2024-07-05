# Correlating Node Centrality Metrics with Node Resilience in Self-healing Systems with Limited Neighbourhood Information.

This repository contains the experimental information developed in the paper  Correlating Node Centrality Metrics with Node Resilience in Self-healing Systems with Limited Neighbourhood Information.

The failure simulator and the self-healing algorithm is implemented in Java at the following link: https://github.com/arleserp/NetworkRecoverySim

## Structure of project 

[selected_networks.gephi](https://github.com/arleserp/CorrelatingNodeCentrality/blob/main/selected_networks.gephi)

Gephi especifications for each graph are here 

[Network specs folder](https://github.com/arleserp/CorrelatingNodeCentrality/tree/main/network_specs)

The folder contains information about the properties of each node in the selected networks:

- closnesscentrality
- eigenvectorcentrality
- degree
- betweenesscentrality
- eccentricity
- pagerank



[Network_global_specs folder](https://github.com/arleserp/CorrelatingNodeCentrality/tree/main/network_global_specs)

Addition of global information related to:

- number of vertices
- number of edges
- Average Path Length
- Clustering coeficients
- Average Clustering Coefficient
- Average degree
- StdDev Average Path Length
- StdDev Degree
- Diameter: 5.0

Experiments organisation:

Due to long size of experiment files they are located in the following links:

Experiment without self-healing (folder exp_0_without_selfhealing): To evaluate the impact of node failures on the networks being tested, we conducted an initial experiment without using the self-healing function. We applied a node failure rate of 𝑝𝑓=0.25.

Experiment minimum number of hops: (folder exp_1_minimum_number_of_hops): The initial experiments aim to determine the minimum number of hops needed to restore a specific network topology. Each node is initially informed about its neighboring nodes within n hops. The probability of node failure at each step is set to 𝑝𝑓=0.25 and 𝑝𝑓=0.125

Memory hop estimation (folder exp_1_2_memory_hop_size_estimation): 
From these results, we could estimate the resource savings (such as memory) achieved by self-healing, which only needs local topology information instead of the entire network. Memory usage is measured in kilobytes and represents the serialisation of topology data for all nodes.

Experiment 2 (folder exp_2_correlation_centrality_vs_node_failure): correlation between centrality metrics and node failure



