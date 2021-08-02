# Honu

[![Go Reference](https://pkg.go.dev/badge/github.com/rotationalio/honu.svg)](https://pkg.go.dev/github.com/rotationalio/honu)
[![Go Report Card](https://goreportcard.com/badge/github.com/rotationalio/honu)](https://goreportcard.com/report/github.com/rotationalio/honu)
![GitHub Actions CI](https://github.com/rotationalio/honu/actions/workflows/build.yaml/badge.svg?branch=main)
[![codecov](https://codecov.io/gh/rotationalio/honu/branch/main/graph/badge.svg?token=7RY96Cu5dx)](https://codecov.io/gh/rotationalio/honu)

**A library for embedded database replication**

## Benchmarks

Baseline comparison of honu database vs. pure leveldb performance to determine the overhead that honu adds:

```
BenchmarkHonuGet-8         	  466665	      2405 ns/op
BenchmarkLevelDBGet-8      	 1243785	       955.3 ns/op
BenchmarkHonuPut-8         	   21448	     55125 ns/op
BenchmarkLevelDBPut-8      	   24276	     52422 ns/op
BenchmarkHonuDelete-8      	   42298	     25136 ns/op
BenchmarkLevelDBDelete-8   	   76857	     16101 ns/op
BenchmarkHonuIter-8        	   63772	     18349 ns/op
BenchmarkLevelDBIter-8     	  255319	      4271 ns/op
BenchmarkHonuObject-8      	  480555	      2362 ns/op
```

[![Baseline Benchmarks](docs/benchmark.png)](docs/benchmark.png)