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
Fixed a bug in [PR #7302](https://github.com/deepspeedai/DeepSpeed/pull/7302) where gradient clipping wasn't working properly with CPU offloading in ZeRO-3. Added unit tests to cover different precision modes and gradient clipping scenarios. 