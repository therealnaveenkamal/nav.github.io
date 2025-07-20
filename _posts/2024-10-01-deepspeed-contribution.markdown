---
layout: post
title:  "Bug Fix: Gradient Norm Calculation for CPU Offload - Microsoft DeepSpeed"
date:   2024-10-01 00:00:00 +00:00
image: /images/deepspeed.jpg
categories: opensource
author: "Naveenraj Kamalakannan"
venue: "Open Source Contribution"
pr: https://github.com/deepspeedai/DeepSpeed/pull/7302
---
Identified and fixed a critical bug in [PR #7302](https://github.com/deepspeedai/DeepSpeed/pull/7302) where gradient clipping modifications were not reflected in global gradient norm calculations when CPU offloading was enabled in ZeRO-3. Implemented comprehensive unit tests covering FP16/BF16 precision modes and various gradient clipping scenarios, ensuring the fix's stability across different configurations. 