# Chapter 5: Cleanroom Logistics, AMHS & Automated Lot Scheduling

## 5.1 Overhead Hoist Transport (OHT) Networks
A $100,000\text{ wpm}$ GigaFab moves tens of thousands of Front Opening Unified Pods (FOUPs)—each carrying 25 wafers—between hundreds of tool bays every day:
- **OHT Rail Systems:** Suspended from the cleanroom ceiling, high-speed automated vehicles travel at $5\text{ m/s}$, picking up and dropping FOUPs onto tool load ports.
- **WIP Storage:** Automated stockers and overhead buffer stations (OHB) temporarily hold wafers between process steps, minimizing queue time.

## 5.2 Little's Law & Cycle Time Management
Total fab cycle time ($CT$) is governed by Little's Law:

$$\text{WIP} = \text{Throughput (TH)} \times \text{Cycle Time (CT)}$$

To reduce wafer turnaround time from 120 days to 90 days without sacrificing throughput, fabs deploy real-time AI dispatching algorithms (dynamic bottleneck scheduling) that route hot lots around tools undergoing preventative maintenance.
