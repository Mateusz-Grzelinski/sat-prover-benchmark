# Prover Benchmark

This project aims to benchmark prover9 and SPASS solvers

## TODO

- add lfg as library

## Dependencies

Provide benchmark script with the following executables: 

- [SPASS](https://www.mpi-inf.mpg.de/departments/automation-of-logic/software/spass-workbench/classic-spass-theorem-prover/download/)
- [prover9](https://www.cs.unm.edu/~mccune/prover9/download/)
- [tptp_to_ladr](https://www.cs.unm.edu/~mccune/prover9/download/) (part of prover9)
- [lfg](https://github.com/Mateusz-Grzelinski/lfg)

You can provice required paths

- by putting them in `PATH`
- by command line arguments
- by setting them in config file

To build dependencies automatically run:

```bash
./scripts/build_deps.sh
```

Script will download and build deps to `lib` folder. Only linux.

### SPASS

Download SPASS 3.9 from [official website](https://www.mpi-inf.mpg.de/departments/automation-of-logic/software/spass-workbench/classic-spass-theorem-prover/download/)

Build with
```shell
make
```

Executable: `lib/spass39/SPASS`

### Prover9 (and tptp_to_ladr)

Download LADR-2009-11A.tar.gz from [official website](https://www.cs.unm.edu/~mccune/prover9/download/)

Build with

```shell
make all
```

Executables: `lib/LADR-2009-11A/bin/prover9`, `lib/LADR-2009-11A/bin/tptp_to_ladr` and more
