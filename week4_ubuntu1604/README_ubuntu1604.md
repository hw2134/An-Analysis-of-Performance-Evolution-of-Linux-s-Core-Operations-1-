# Week4 Experiment: Ubuntu16.04 VirtualBox VM
## Goal
Reproduce the baseline kernel v4.0.5 and kernel v4.15.0-112 from the paper Figure 1.
- v4.0.5: baseline, without KPTI / Spectre mitigations
- v4.15.0-112: kernel with KPTI + Retpoline security patches

## Environment
- Hypervisor: Oracle VirtualBox
- Guest OS: Ubuntu 16.04
- Benchmark: LEBench / OS_Eval
- Kernel 1: 4.0.5-040005-generic
- Kernel 2: 4.15.0-112-generic

## Status
Boot successfully
OS_Eval completed, CSV output generated

## Run command
```bash
cd ~/LEBench
./OS_Eval
# After run, rename csv to avoid overwrite
cp output.4.0.5-040005-generic.csv raw_csv/output.4.0.5-040005-generic_run1.csv
