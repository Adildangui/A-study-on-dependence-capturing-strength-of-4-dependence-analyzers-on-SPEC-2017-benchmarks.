A Study on "Dependence capturing strength" of 
four Dependence Analyzers in LLVM on SPEC 2017 benchmarks
=======================================================================================================

## **Adil Arun Dangui, Utpal Bora, Dangeti Tharun Kumar**
## **IIT HYDERABAD**

In this project, we study the "dependence capturing strength" of the four dependence analyzers on SPEC 2017 benchmarks. Namely the following

1.  Loop Access Info (LAI)

2.  Dependence Analysis (Goff, Kennedy, Tseng)

3.  Memory Dependence Analysis

4.  Polly's Dependence Analyzer ()

Getting Started:

--------------------

### LLVM:

The LLVM compiler infrastructure project is a "collection of modular and reusable[  ](https://en.wikipedia.org/wiki/Compiler)compiler and[  ](https://en.wikipedia.org/wiki/Toolchain)toolchain technologies" used to develop compiler[  ](https://en.wikipedia.org/wiki/Compiler#Front_end)front ends and[  ](https://en.wikipedia.org/wiki/Compiler#Back_end)back ends.

LLVM has three dependence analyzers for capturing dependencies. LAI is used on large scale by llvm for dependence capturing which in turn is used for optimizations. Goff-kennedy and Memory dependence analysis are other two analyzers in llvm.

### Polly:

Polly is a high-level loop and data-locality optimizer and optimization infrastructure for LLVM. It uses integer polyhedral model of the code and based on it tries to analyze and make optimizations in memory access patterns. Polly is capable of doing advanced loop transformations, tiling, vectorization etc. Polly has also displayed its optimization strength by showing massive runtime improvement over certain codes which were otherwise relatively slower. The Polyhedral optimization framework enables modeling of arbitrarily complex sequence of loop transformations into a single optimization step.

Polly has its own dependence analyzer which runs as a polly pass and facilitates Polyhedral optimizations.

### SPEC-2017:

It is a collection of standardized benchmarks and tools to evaluate performance and energy efficiency of computer systems. In this study however we'll be focusing only on following benchmarks.

[500.perlbench_r](https://www.spec.org/cpu2017/Docs/benchmarks/500.perlbench_r.html), [502.gcc_r](https://www.spec.org/cpu2017/Docs/benchmarks/502.gcc_r.html), [505.mcf_r](https://www.spec.org/cpu2017/Docs/benchmarks/505.mcf_r.html), [523.xalancbmk_r](https://www.spec.org/cpu2017/Docs/benchmarks/523.xalancbmk_r.html), [531.deepsjeng_r](https://www.spec.org/cpu2017/Docs/benchmarks/531.deepsjeng_r.html), [541.leela_r](https://www.spec.org/cpu2017/Docs/benchmarks/541.leela_r.html), [548.exchange2_r](https://www.spec.org/cpu2017/Docs/benchmarks/548.exchange2_r.html), [508.namd_r](https://www.spec.org/cpu2017/Docs/benchmarks/508.namd_r.html), [510.parest_r](https://www.spec.org/cpu2017/Docs/benchmarks/510.parest_r.html) , [544.nab_r](https://www.spec.org/cpu2017/Docs/benchmarks/544.nab_r.html).

## Prerequisites:

------------------

1.  Prerequisite passes:

Following passes were run before getting the the count of dependencies captured by each analyzer.

-mem2reg  -loops  -loop-simplify  -loop-rotate  -loop-simplifycfg

## Results:
------------------

 <https://drive.google.com/open?id=1Sgfpe7D3t2j_COj0C4NJMNdlxGSuj8Qw>
