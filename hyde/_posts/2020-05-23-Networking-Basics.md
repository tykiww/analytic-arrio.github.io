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

<hr>

<iframe width="560" height="315" src="https://www.youtube.com/embed/1R0UgIgcb5g" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<hr>

<iframe width="560" height="315" src="https://www.youtube.com/embed/lHmFRlETTcQ" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<hr>

### Networking Multi-Node Motherboards

Here are THE ONLY examples I could find on how others have created a multi-gpu system for deep learning. 

NVIDIA:

How to..

- https://devblogs.nvidia.com/how-build-gpu-accelerated-research-cluster/


Tim Dettmers:

- https://timdettmers.com/2014/09/21/how-to-build-and-use-a-multi-gpu-system-for-deep-learning/

More on CUDA aware MPI: https://developer.nvidia.com/mpi-solutions-gpus

Honestly, I think TD's instructions and comments at the bottom are the most clear. Our real question is whether to use a bonded PCI port and some (insert number here)Gb switch OR buying HCInfiniband cards and cables. The port and switch is closer to the raspberry pi example above. However, from the reading above, it seems like doing the HCI cards provide cheaper (take a look at how much a 40gb switch costs..) communication without too much latency. I honestly cannot think of our analytics group even needing more than 2 deep learning specialists anyways, so I would even venture to store data on NVMEs without a switch because after the initial transport of data to the node, computation is just as fast.


### Configuration and Software Scheduling

This part is very hazy for me. This will be more exploratory once we can get everything to boot up!

From here, we will be exploring without much previous help!

This link was very helpful for me to realize that there is some merit to thinking about how to connect the gpu interface. On a sidenote, we really don't need NVLink. We're not going that crazy on GPU-GPU communication. the PCI express connections should be good enough for our use case. 

- https://lambdalabs.com/blog/introduction-multi-gpu-multi-node-distributed-training-nccl-2-0/

This is more on the scheduling side. We'll get to that as it comes. Shouldn't really be that challenging, right? lol.

- https://guiesbibtic.upf.edu/recerca/hpc/multi-node-multi-gpu






