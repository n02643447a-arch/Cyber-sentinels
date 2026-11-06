name: GIJIMA MANNERS
REG NUM: N02640778M
CONTRIBUTION: RESEARCH CPU AND MEMORY MONITORING

CPU and Memory Monitoring with eBPF
1. What is It?
eBPF runs small, super-fast security and tracking programs directly inside the Linux kernel. It tracks how your computer uses its CPU (processor) and Memory without slowing down your system.
2. How It Works
CPU Monitoring: Tracks which apps use the processor, how long tasks wait to run, and what threads do when they are paused (off-CPU time).
Memory Monitoring: Tracks when memory is requested or freed (malloc/free), detects memory leaks, and catches page faults instantly.
3. Why Use eBPF Instead of Old Tools?
Near-Zero Overhead: Runs inside the kernel instead of constantly checking apps from the outside 
Extreme Accuracy: Catches quick resource spikes that traditional tools miss.
Clear Context: Links every CPU or memory spike to the exact app, process, or container causing it.
4. Quick Tool Checklist
profile: Pinpoints which line of code is using up the CPU.
off-cputime: Shows why an app is waiting or frozen off the CPU.
memleak: Finds un-freed memory to fix memory leaks.
perf: Measures general system and kernel performance.
