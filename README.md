# vasp_benchmark
Benchmark test for checking PC speed using VASP code.

# Small calculation
#### Calculatoin: Structure optimization of wurtzite-ZnO using VASP. 

| option | values |  
| ---- | ---- |
| ZnO supercell | Zn\*2, O\*2|  
| Cutoff | 500eV |
| EDIFF | 0.0001 |
| kpt | 7x7x4 |
| EDIFFG | 0.0001 |
| ISIF | 3  |

#### Results
| CPU  | # of parallel | Elapsed time (sec) | Compiler, Library, etc. |  VASP version |
| ---- | ---- |---- |---- |---- |
| Pentium 4 3.0GHz  | 1 | 405.700	| MKL |  VASP.4.6.12 |
| Pentium D 2.8GHz  | 2 | 175.061 | ATLAS | VASP.4.6.12 |
| Pentium D 2.8GHz  | 2 | 145.897 | MKL | VASP.4.6.31| 
| Athlon 4.4+GHz  | 2 | 157.976	 | ATLAS | VASP.4.6.12| 
| Core2Duo 2.4GHz  | 2 |103. | MKL | VASP.4.6.12| 
| Core2Quad 2.4GHz  | 4 | 107.071 | MKL | VASP.4.6.28| 
| Core2Quad 2.4GHz  | 4 | 98.455 | MKL | VASP.4.6.28| 
| Core2Quad 2.4GHz  | 4 | 89.891 | MKL | VASP.4.6.28| 



# Large calculation



