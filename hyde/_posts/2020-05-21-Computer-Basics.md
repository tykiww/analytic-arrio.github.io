---
layout: post
title: Introducing Hyde
description: >
  Useful general information on Computer parts
author: Tyki
noindex: true
---


### Understanding Basic Computer Parts

General Basics

<iframe width="560" height="315" src="https://www.youtube.com/embed/ExxFxD4OSZ0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Can be confusing to understand the use of PCI express lanes. A good retro video to understand its purpose.

<iframe width="560" height="315" src="https://www.youtube.com/embed/PrXwe21biJo" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Another PCIe Lane explanation

<iframe width="560" height="315" src="https://www.youtube.com/watch?v=LSSHuMHbCWo" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


Kind of a funny video, but is a useful explanation on the purpose of a GPU. More on that later.

<iframe width="560" height="315" src="https://www.youtube.com/watch?v=6stDhEA0wFQ" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Understanding Deep Learning Hardware

This [page](https://timdettmers.com/2018/12/16/deep-learning-hardware-guide/) is probably the staple for all gpu computing clustering

##### TL;DR (Directly taken from page)

- *GPU:* RTX 2070 or RTX 2080 Ti. GTX 1070, GTX 1080, GTX 1070 Ti, and GTX 1080 Ti from eBay are good too!

- *CPU:* 1-2 cores per GPU depending how you preprocess data. > 2GHz; CPU should support the number of GPUs that you want to run. PCIe lanes do not matter.

- *RAM:*

  1) Clock rates do not matter — buy the cheapest RAM.
  2) Buy at least as much CPU RAM to match the RAM of your largest GPU.
  3) Buy more RAM only when needed.
  4) More RAM can be useful if you frequently work with large datasets.

- *Hard drive/SSD:*
  1) Hard drive for data (>= 3TB)
  2) Use SSD for comfort and preprocessing small datasets.

- *PSU:*
  1) Add up watts of GPUs + CPU. Then multiply the total by 110% for required Wattage.
  2) Get a high efficiency rating if you use a multiple GPUs.
  3) Make sure the PSU has enough PCIe connectors (6+8pins)

- *Cooling:*
  1) CPU: get standard CPU cooler or all-in-one (AIO) water cooling solution
  2) GPU:
  3) Use air cooling
  4) Get GPUs with “blower-style” fans if you buy multiple GPUs
  5) Set coolbits flag in your Xorg config to control fan speeds

- Motherboard:
  1) Get as many PCIe slots as you need for your (future) GPUs ~~(one GPU takes two slots; max 4 GPUs per system)~~

- Monitors:
  1) An additional monitor might make you more productive than an additional GPU.





