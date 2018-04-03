## cache (cash) miss
* cold miss - the cache is empty, transient states before the warming up.
* conflict miss - the hardware restricts a particular block at k+1 level to a small subset of the blocks at k level. Even the cache is not full, some blocks in the working set can not be fetched to that empty position.
* capacity miss - the cache size is not large enough.

## locality
```c
int sumvec(int vN[]) {
  int i, sum = 0;
  for (i = 0; i < N; i++)
    sum += v[i];
  return sum;
}
```
* spatial locality - if a memory location is referenced once, then the program is likely to reference a nearbby memory loaction in the near future.

* temporal locality - a memory location that is referenced once is likely to be referenced again in the near future, like sum

* the example is a stride-1 pattern.
