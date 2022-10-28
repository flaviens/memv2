# Trying to break down this $mem_v2 without success

## How to reproduce

I'm using the Yosys commit `fc53a0a5c213dd1b51a3303fa90f46954d4a9664` on Ubuntu 22.06

```
git clone https://github.com/flaviens/memv2
cd memv2
make
```

## Output

```
=== bram_model ===

   Number of wires:                 29
   Number of wire bits:            146
   Number of public wires:          17
   Number of public wire bits:      78
   Number of memories:               0
   Number of memory bits:            0
   Number of processes:              0
   Number of cells:                 13
     $mem_v2                         1
     $mux                           12
```

But I'd like to break down mem_v2 into standard cells and DFFs, like the `mem` pass does for some other memories.
