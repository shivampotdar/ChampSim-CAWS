
### src/cache.cc
1. Indent whole file for if-related warnings


### src/main.cc
1. 317: Function should return uint64_t and not char
2. 330: page_table.end**()**
3. 339: begin**()** and end**()**
4. 351: end**()**
5. 360: erase
6. 361: insert
7. 430: insert
8. 457: end**()**
9. 338: delete or comment as variable pr2 is not used
10. 1: change to DEFAULT_SOURCE as _BSD_SOURCE is deprecated

### src/ooo_cpu.cc
1. Indent whole file for if-related warnings
2. 1858: delete or comment as variable instruction_physical_address is not used

### prefetcher/no.(l1d,l1i,l2c,llc)_pref 
1. remove that var, literally ;)

### For the exercise

- Pin 3.2 is not compatible with Ubuntu 20.04 (Linux 5.0). After numerous attempts of playing around with parameters like -injection and recompiling the .so files, and trying on different systems with Ubuntu 18.04 and AMI Linux (AWS EC2), I finally upgraded to Pin 3.17 (https://software.intel.com/sites/landingpage/pintool/downloads/pin-3.17-98314-g0c048d619-gcc-linux.tar.gz) and then refactored the `champsim_tracer.cpp` file to work with the new version.

- With this change, the trace and simulation runs successfully.

- IPC value 1.11995
