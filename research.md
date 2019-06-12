---
title: Research
layout: page
permalink: /research/
---

[Current Projects](#current) <br> [Past Projects](#past)

The RSSL conducts research in a number of different areas, broadly related to computer engineering, computer architecture, embedded systems, fault tolerance and reliability, security, and machine learning. 
Most research at RSSL combines some set of system architecture, system modeling, and optimization.

<a name="current"></a>
# Current Projects

## Hardware-Software Optimization of Machine Learning Algorithms

Artificial neural networks (ANN), historically used in machine learning to solve classification problems, are beginning to appear in a wide variety of applications domains, such as modeling, decision making, data processing, robotics, and control. 
Conventionally, ANN are designed for classification accuracy, and the more the better, but the resulting systems are often large and expensive, unsuitable for low-cost applications.
Furthermore, until recently, ANN optimization was a laborious, manual process.

Our research in this area includes automated optimization of neural networks (using sequential model-based optimization), and other techniques. 

## VoltSpot: Power-delivery Network Modeling and Optimization

In future CMOS technology nodes, threshold and supply voltages are not scaling down as fast as device density is increasing.
Higher current density and total current place greater demands on the power-delivery network (PDN); current-related chip phenomena such as electromigration (EM), resistive current (IR) drop, and inductive transient current (Ldi/dt) noise all get worse with higher current and larger current swings.
[VoltSpot](http://lava.cs.virginia.edu/VoltSpot/) is an architecture-level model of the on-chip PDN including C4 pads, with a simple interface for use in other architecture-level tools. 
VoltSpot, when integrated with a performance simulator (such as gem5) and power estimation tool (such as McPAT), provides architects with the tools necessary to explore the effect of PDN design, including C4 pad allocation to VDD, GND and I/O and PDN metal width. 
VoltSpot also supports the exploration of run-time IR drop and Ldi/dt noise prediction, avoidance, and mitigation.  
Recent work has begun to explore design techniques for system lifetime, 3D-ICs and simulation techniques for accelerating the process of solving for on-chip voltage noise.

<a name="past"></a>
# Past Projects

## ArchFP: Architectural Floorplanning for Early Design Analysis

[ArchFP](http://lava.cs.virginia.edu/archfp/index.htm) is a simple, easy to use, architect-directed floorplanning tool. Floorplanning tools grew out of a need to automate the placement of standard cells and module in large, complex designs. 
Floorplans are often needed in order to estimate design area, performance, power, temperature, and therefore reliability. 
System architects need a way to generate floorplans for the same reason but system-level floorplans, which often consist of only a handful of blocks, often placed in some regular way (e.g., tiled cores), are poorly explored by tools designed to manage the complexity of thousands of blocks. 
ArchFP gives a system architect a tool that leverages their knowledge of the system and quickly produces a floorplan that can be used for further analysis.

## Design-space Exploration for Embedded MPSoCs

Embedded system designers rely on automation approaches to meet time-to-market constraints, but to date few tools have been developed to assist with optimizing system cost, lifetime. 
To this end, we have developed (a) techniques to accelerate lifetime estimation and (b) lifetime-aware design space exploration. 
Earlier, we developed a system synthesis approach that, given an application, hardware/software partitioning and communication architecture, selects and organizes system resources, allocating and distributing slack to jointly optimize system cost and lifetime. 
Additional research has explored the effect of task mapping on lifetime in this context. 
Recently, we have developed novel models for abstracting behavior observed in atomistic models of negative-bias temperature instability to the level of standard cell libraries.  
Other work explore a new approaches to quickly estimating system lifetime using multi-armed bandits.

## Internet Packet Classification

ISPs and network administrators use Internet Packet Classification (IPC) to categorize packets into flows (traffic sharing IP addresses, ports, and protocol), and thereby the application classes generating them. Distinguishing between safe and malicious traffic aids in network intrusion interception. 
Likewise, categorizing applications into classes is useful for traffic management for better service. 
Traditional IPC based on port numbers and payload pattern recognition are no longer effective because current applications can dynamically change port numbers and cipher their contents. 
Recent machine learning (ML) IPC solutions have speed-bounded accuracy, and complex implementation due to their dependence on packet sizes and order of arrival. 
We propose a new IPC approach that uses associative memory (AM) based on sparse-clustered network with selective decoding, dramatically reducing the memory for hardware implementation of IPC, while significantly improving classification throughput.

## Yield Improvement for Parallel Architectures

Recent research as suggested that as more processor cores are incorporated on single chips, the appropriate granularity of redundancy for the purpose of failure and defect mitigation is at the system-level. 
We leverage this fact above, but have observed that some systems benefit from a combination of system-level and microarchitetural redundancy. 
In this project, we investigate the relationship between parallel application, parallel architecture (and single-instruction, multiple-thread architectures in particular), and redundancy allocation, based on the observation that as the demand for types of parallel resources changes (e.g., from many narrow cores to few wide cores), so ought the mix of redundant components (e.g., from redundant cores to cores with redundant lanes).

