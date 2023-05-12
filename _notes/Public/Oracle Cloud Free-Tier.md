---
title: Oracle Cloud Free-Tier
feed: show
date: 05-05-2023
permalink: /oracle-cloud-free-tier
---

Oracle Cloud offers several free servers for developers -  2 AMD-based Compute VMs (with 1/8 OCPU and 1 GB memory each) and ARM-based Ampere A1 cores with 24 GB of memory (usable as 1 VM or up to 4 VMs with 3,000 OCPU hours and 18,000 GB hours per month).
[What's also included with Oracle Cloud Free Tier](https://www.oracle.com/cloud/free/).

I used them before, but for now for my learning I decided to configure it again and write about it here.

So I am configuring 1 ARM-based and 2 AMD-based VMs.

## VM1: 4 ARM-based Ampere A1 cores + 24 GB of memory

I am using Canonical Ubuntu 22.04 (I prefer to use standard image instead of minimal one) as an image and VM.Standard.A1.Flex as a shape (Virtual machine, 4 core OCPU, 24 GB memory, 4 Gbps network bandwidth).

I created a public key file `is_rsa_oracle.pub` with the `ssh-keygen` command from my laptop and added this SSH key to the instance.

And also I am using boot volume size of 100 GB (of 200 GB available in free-tier).





Tags: #Oracle, #free