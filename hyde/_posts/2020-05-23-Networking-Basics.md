---
layout: post
title: HPC Networking Basics
description: >
  Most Crucial Part of the Project.
author: Tyki
noindex: true
---

This is probably where the money is at. 


### Basic Networking

This is very low-level, using Raspberry Pis, but this video series may help visualize what we are doing. 
However, in no way are we going to use mpich. We need to use some CUDA aware MPI, so bear that in mind as you watch.

1
https://www.youtube.com/watch?v=1R0UgIgcb5g
2
https://www.youtube.com/watch?v=lHmFRlETTcQ

### Networking Multi-Node Motherboards

Our real question is whether to use a bonded PCI port and (insert number here)Gb switch OR buying HCInfiniband cards and cables.

Here are some examples on how others have created a multi-gpu system for deep learning.

NVIDIA:

How to..

- https://devblogs.nvidia.com/how-build-gpu-accelerated-research-cluster/



Tim Dettmers:

- https://timdettmers.com/2014/09/21/how-to-build-and-use-a-multi-gpu-system-for-deep-learning/

More on CUDA aware MPI: https://developer.nvidia.com/mpi-solutions-gpus



### Software Scheduling

This part is very hazy for me. This will be more exploratory once we can get everything to boot up!

From here, we will be exploring without much help!

- https://lambdalabs.com/blog/introduction-multi-gpu-multi-node-distributed-training-nccl-2-0/
- https://guiesbibtic.upf.edu/recerca/hpc/multi-node-multi-gpu






