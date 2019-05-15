# FastR vs R - Profiling Results

Basic performance test between standard R and Graal's FastR. Run on 2019-05-15
Preliminary results point to FastR being slower than standard R for this benchmark.

## Graal FastR
* GraalVM CE 19.0.0 
* FastR installed via `$GRAALVM_HOME/bin/gu install R`

## Native R
* v3.6.0
* Installed from https://cran.ma.imperial.ac.uk/
* https://cran.ma.imperial.ac.uk/bin/macosx/R-3.6.0.pkg

## Benchmark
R benchmark copied from https://mac.r-project.org/benchmarks/bench.R

* Native R: `R --no-save < benchmark.R > raw_R_result.txt`
* Graal FastR: `$GRAALVM_HOME/bin/R --no-save < benchmark.R > fastR_result.txt` 

## Benchmark 2
R benchmark copied from https://mac.r-project.org/benchmarks/bench.R

* Native R: `R --no-save < benchmark_v2.R > raw_R_result_v2.txt`
* Graal FastR: `$GRAALVM_HOME/bin/R --no-save < benchmark_v2.R > fastR_result_v2.txt` 

## Machine Details

* MacBook Pro
* macOS Mojave 10.14.4
* Intel Core i7 2.2 GHz
* 16GB 1600 MHz DDR3