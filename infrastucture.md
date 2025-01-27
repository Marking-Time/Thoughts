[back to Thoughts](https://github.com/Marking-Time/Thoughts/tree/main)
1/27/2025
# Infrastructure  

Much has been written about the vulnerabilities of the technical infrastructure that we rely on for daily life. Everything from power grids, water supplies and even traffic lights are vulnerable to cyber attack. Much of this is because the infrastructure is old and needs to be updated.

### The Problem
These systems do simple things.  They open and close valves, time how long something has been running, or do simple logic like > if valve "a" and valve "b" are open then close valve "c" else open valve "c". They don't require complex logic or modern chips.  They relied on simple 4 bit processors that date to the mid 1970s. The systems may be simple, but they perform very important tasks.  Often it would require a highly trained human operator to replace them. The failure of these systems can cerate catastrophic consequences.

The infrastructure is old.  Some of it predates modern semiconductors and has been upgraded and modified as technology progressed.  Often the software relies on proprietary code written in languages that were state of the art at the time, but have since fallen out of use in favor of languages and techniques  that have more power and are easier to use.  

Over time, the systems have been improved by layering on technologies like control systems and network connectivity, while still using the simple chips and logic that actually do the work of causing the valve open or close. The systems work, but they have vulnerabilities based largely based on their complexity.  

A partial list of problems:
- The chips are not manufactured in the US because the old chips are low margin and don't require modern manufacturing techniques or tooling.
- The code that runs the entire stack including, the simple processors that operate the valves, the system control and monitoring software and the network connectivity often use proprietary code.  There are "silos" of knowledge held by people that retired 20 years ago. This make the system difficult to audit. 
- Because of the above the documentation needed to keep the system operating is incomplete or missing.  This leads to "patches" and "workarounds" that add more complexity to the system.

### A Solution  
Because of the critical nature of these systems the entire stack including hardware and software needs to be open source and become a national standard. It should be simple for an engineer to find the documentation necessary to repair or upgrade a system. 

To make the systems more secure and to have a reliable supply chain, the chips should be manufactured in the US by companies like Texas Instruments which already own the designs for these chips and have amortized the design costs decades ago.  A family of chips like the [TI TMS1000](https://en.wikipedia.org/wiki/Texas_Instruments_TMS1000) would be a good starting point (you know your famous when you get your own wikipedia page).  

The software should also be an open source national standard. This would make the system easier to troubleshoot and upgrade.

These physical systems can still break, but at least the replacement parts would not be vulnerable to international supply chains. 






