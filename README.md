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

## Workbook Structure and Model-Parameter Mapping

All 30 benchmark workbooks follow the same standardized worksheet structure. Except for the `Results` worksheet, each sheet defines one family of input parameters used by the mathematical and CP models. The data are stored in long format: the first columns identify the relevant indices, while the `val` column contains the numerical parameter value.

The worksheet names correspond to those used by the Python data-loading functions. Where a worksheet name differs from the notation used in the manuscript, the corresponding manuscript parameter is also reported below.

| Worksheet | Manuscript parameter       | Columns                        |
| --------- | -------------------------- | ------------------------------ |
| `scalars` | Sets and scalar parameters | `name`, `val`                  |
| `ar`      | (ar_i)                     | `i`, `val`                     |
| `arp`     | (ao_k)                     | `k`, `val`                     |
| `H`       | (hi_{pi})                  | `p`, `i`, `val`                |
| `Hp`      | (h_{pk})                   | `p`, `k`, `val`                |
| `tt`      | (t_{jm})                   | `j`, `m`, `val`                |
| `ttp`     | (tl_{ml})                  | `m`, `l`, `val`                |
| `op`      | (o_{pmg})                  | `p`, `m`, `g`, `val`           |
| `pr`      | (pr_{pmg})                 | `p`, `m`, `g`, `val`           |
| `st`      | (st_{g_1g_2m})             | `m`, `g`, `gt`, `val`          |
| `zp`      | (pd_{pik})                 | `p`, `i`, `k`, `val`           |
| `Results` | Computational output       | Method and performance columns |


## Reported Computational Results

Each Excel workbook also reports the following information, where applicable:

* Best objective value
* Best bound
* Solution time in seconds
* Time to best solution
* Optimality gap
* Solver status

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
