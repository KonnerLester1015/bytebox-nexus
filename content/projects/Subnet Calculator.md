---
title: "Subnet Calculator"
sidebar:
  exclude: true
---
## Introduction

This document provides background information on the purpose and usage of this subnet calculator. I created this subnet calculator while taking a Network Fundamentals course at Purdue University. The course included several "subnetting assignments" that required performing calculations using a host IP address, a major network mask, and a subnet mask. 

Using these inputs, I then had to perform bitwise operations to determine several pieces of information, as outlined in Table 1.

**Table 1 - Example Subnet Sheet**

|   Variable | Example Value  |
|--------|------|
|    Host IP Address | 219.2.3.201   |
|  Major Network Mask | 255.255.0.0   |
|  Major Ntwork Address | 219.2.0.0  |
|  Major Network Broadcast Address | 219.2.255.255   |
|  CIDR Notation Major Network | 219.2.0.0/16   |
|  Number of Host Bits | 16   |
|  Number of Hosts | 65,534   |
