# Lifish

Lifish is a Light chess engine based on StockFish.

List of removed features in Lifish:

* Syzygy

* Chess960

* Skill Level

* ...

###


## UCI parameters

Currently, Lifish has the following UCI options:

  * #### Threads
    The number of CPU threads used for searching a position. For best performance, set
    this equal to the number of CPU cores available.

  * #### Hash
    The size of the hash table in MB.

  * #### MultiPV
    Output the N best lines (principal variations, PVs) when searching. Leave at 1 for best performance.

  * #### Move Overhead
    Assume a time delay of x ms due to network and GUI overheads. This is useful to avoid losses on time in those cases.

## Compiling Lifish

The [MSYS2](https://www.msys2.org/) environment is recommended for compiling Lifish on Windows.

To compile, type:

    make target ARCH=arch [COMP=comp]

Example: `make build ARCH=x86-64 COMP=mingw`

Lists of supported targets, archs and compilers can be viewed by typing `make help`.
