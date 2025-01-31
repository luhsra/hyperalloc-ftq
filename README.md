# HyperAlloc: FTQ Benchmark

This benchmark is a modified version of the [FTQ benchmerk](https://asc.llnl.gov/coral-benchmarks) for the HyperAlloc paper.

- See: https://github.com/luhsra/hyperalloc-bench

## Publication

HyperAlloc: Efficient VM Memory De/Inflation via Hypervisor-Shared Page-Frame Allocators
Lars Wrenger, Kenny Albes, Marco Wurps, Christian Dietrich, Daniel Lohmann
In: Proceedings of the 20th European Conference on Computer Systems (EuroSys 2025); ACM

## ftq

Run `make ftq; make t_ftq` to build. This produces two binaries one for single threaded and one for multi threaded use.
For info on running the benches, see the `summary.pdf`.

A run will produce two files (per core) which contain the timestamps and work ammounts respectively. For multi threaded runs
these are broken however. The fixed version writes the correct data to two extra files `[times,counts].dat`. These contain the
the measurements for all cores one after another.
