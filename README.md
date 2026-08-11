# Cross-dock-reconfigurable-machines-benchmarks
Benchmark instances and detailed computational results for “A cross-dock scheduling problem with reconfigurable process machines: A constraint programming approach.”
# Cross-Dock Scheduling with Reconfigurable Process Machines: Benchmark Instances and Computational Results

This repository contains the benchmark instances and detailed instance-level computational results associated with the manuscript:

The repository is intended to facilitate transparent comparison, validation, and future benchmarking of solution methods developed for the studied cross-dock scheduling problem.

## Repository Contents

| File                | Description                                                                                 |
| ------------------- | ------------------------------------------------------------------------------------------- |
| `benchmark-instances.zip`    | Contains the 30 benchmark instances used in the computational experiments.                  |
| `README.md`         | Describes the benchmark data, computational results, and experimental settings.             |

## Benchmark Instances

The benchmark set consists of 30 instances named `sample_01.xlsx` through `sample_30.xlsx`. The instances are divided into three groups of increasing size:

* Instances 01–10: small-sized instances
* Instances 11–20: medium-sized instances
* Instances 21–30: large-sized instances

## Reported Computational Results

Each Excel workbook also reports the following information, where applicable:

* Best objective value
* Best bound
* Solution time in seconds
* Time to best solution
* Optimality gap
* Solver status, such as `Optimal` or `Time Limit`

## Computational Environment

The experiments were conducted using the following system:

| Item                    | Specification                                |
| ----------------------- | -------------------------------------------- |
| Processor               | Intel Core i7-1165G7                         |
| Operating system        | Windows 10, version 22H2, 64-bit (OS build 19045)|
| Programming language    | Python 3.10.0                                |
| MILP modeling framework | Pyomo 6.10.1                                 |
| MILP solver             | IBM ILOG CPLEX 22.1.0.0                      |
| CP modeling interface   | DOcplex.CP 2.32.264                          |
| CP solver               | IBM ILOG CP Optimizer 22.1.0.0               |
| Main time limit         | 600s for small-sized instances, 1800s for medium-sized instances, 3600s for large-sized instances   |

The same computational conditions and stopping criteria were applied to the compared formulations for each benchmark instance.

## Citation

If you use these benchmark instances or computational results, please cite the associated article. The complete bibliographic information will be added after publication.

Repository URL:

https://github.com/mohammadtavakkoli/cross-dock-reconfigurable-machines-benchmarks
