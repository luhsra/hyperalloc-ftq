# ftq

Run `make ftq; make ftq_t` to build. This produces two binaries one for single threaded and one for multi threaded use.
For info on running the benches, see the `summary.pdf`.

A run will produce two files (per core) which contain the timestamps and work ammounts respectively. For multi threaded runs
these are broken however. The fixed version writes the correct data to two extra files `[times,counts].dat`. These contain the
the measurements for all cores one after another.
