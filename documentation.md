---
title: Documentation
---

## Hardware Requirements

GraphSense can process hundreds of millions transactions from several ledgers and is therefore built on-top of [Apache Spark](spark) and [Cassandra](cassandra).

In our production environment we use a Apache Spark/Cassandra cluster with the following Hardware components:

* 1 master node: DELL PowerEdge R740, 2×Intel Xeon 2.60GHz (14 cores), 320 GB RAM, 3×4TB HDD (Raid 5), 2×512GB SSD (Raid 0)

* 8 worker nodes: Supermicro 815TQC-R501WB, 2×Intel Xeon 1.7 GHz (6 cores), 256GB RAM, 4TB HDD, 3×2TB SSD

All nodes are connected via **10Gbit ethernet** interfaces and a corresponding switch. With this setup the computation time to create the address and entity graph using the transformation component is currently ~13h for Bitcoin.

In our previous setup we used just four worker nodes, which can be seen as minimal requirement to run the transformation pipeline for larger blockchains like Bitcoin.

## Setting up GraphSense

TBD.



[spark]: https://spark.apache.org/
[cassandra]: https://cassandra.apache.org/
