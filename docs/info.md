<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works

![Block Diagram](Block_Diagram_Alt_v1.png "Block Diagram")

## How to test

Table of I/O Assignments

| Internal Mapping | Pin Mapping | I/O |
| ---------------- | ----------- | --- |
| Data Bus Out [7:0] | Out [7:0] | Out - Output of CPU |
| Data Bus In [7:0] | In [7:0] | In - Take in instruction from test script |
| PC | I/O [7:4] | Out - Send to test script for correct instruction |
| Instruction Enable | I/O [3] | Out - Tells test script to send instruction |
| Clk | I/O [2] | In - clock for CPU controlled by test script |
| RST' | I/O [1] | In - Resets PC |
| Status | I/O [0] | Out - Tells status of CPU (active, error) |

## External hardware

List external hardware used in your project (e.g. PMOD, LED display, etc), if any
