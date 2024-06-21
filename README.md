# Integrity Managament in Graph Databases using E/R keys

## Introduction: 

This Github repository complements our research on integrity management in graph databases using E/R keys.

In particular, this repository is comprised of the following:

- experiment results on the TPC-H benchamrk
- compilations that outline how experiments have been conducted
- images illustrating the experiments on graph datasets
- files and instructions on how to replicate experiments and shwoing their results

## Preliminaries:

The software used to perform the experiments carried out in our research are:

- Neo4j Desktop 1.5.0

- Neo4j Browser 5.0.0


The TPC-H benchmark is provided on the official [TPC website](https://www.tpc.org/tpch/). 


## Experiments:

The experiments in our research on E/R keys are outlined in the following:

- 1.) [How can E/R keys improve entity integrity management?](https://github.com/GraphDatabaseExperiments/integrity_experiments/tree/main/entity_integrity)
- 2.) [How can E/R keys improve referential integrity management?](https://github.com/GraphDatabaseExperiments/integrity_experiments/tree/main/referential_integrity)


Detailed information on the results of these experiments and instructions on how to replicate them can be found in this repository in the experiments folder or by clicking on the links above. In what follows we like to provide an overview on the different experiments.

### 1.) Entity Integrity

We highlighted the benefits of E/R keys enforced on E/R graphs by manually checking whether a respective key O(C,K) is satisfied on graph translation of TPC-H under relational, mixed and graph semantics. For this we executed queries that output vioalations of the corresponding keys.

### 2.) Referential Integrity

The benefits of our modelling approach with respect to referential integrity management has been shown through the execution of update propagations. Here, we updated properties on nodes that might require updates of the same property on differenlty labelled nodes where they serve as foreign key in TPC-H. For the same property this might result in a different update propagation depending on whether TPC-H had been modelled adhering to relational, mixed or graph semantics.

Text missing


