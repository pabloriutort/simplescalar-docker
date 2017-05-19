simplescalar-docker
===

This is a fork of the simplescalar-docker to implement a DRAM-Simulator

## simplescalar
Instructions from http://www.cse.iitd.ernet.in/~cs5070217/csl718/assignment1/ss_install_instructions.html

## DRAM-Simulator
There is a [DRAM Simulator](https://github.com/pabloriutort/DRAM-Simulator/tree/master) git submodule into [simplescalar-docker/simplesim-3.0/DRAM](https://github.com/pabloriutort/simplescalar-docker/tree/master/simplesim-3.0)

### Usage

1. Excute the python script into simplesim-3.0/DRAM folder called `dram.py`
  ```
  ./dram.py
  ```
2. Execute the `run` script into simplesim-3.0
  ```
  ./run <configuration> <simulator> <path of tests or benchmarks>
  ```
  Example:
  ```
  ./run alpha sim-outorder tests-alpha/bin/test-math
  ```
  This will compile and run the math tests in `sim-outorder` with `alpha` config. Next time we might execute just:
  ```
  ./sim-outorder tests-alpha/bin/test-math
  ```
  Because sim-outorder is "alpha compiled".

  Another example could be execute some benchamrks into the benchmark folder
  ```
  ./run alpha sim-outorder ../benchmark/<benchmark configuration>
  ```
3. Wait for the end of execution or stop it manually.

More info about DRAM-Simulator in [its wiki](https://github.com/pabloriutort/DRAM-Simulator/wiki)
