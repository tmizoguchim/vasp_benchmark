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
| Download .tar file | http://www.edge.iis.u-tokyo.ac.jp/vasp/speed-chk-small.tar  |

#### Results
| CPU  | # of parallel | Elapsed time (sec) | Compiler, Library, etc. |  VASP version | # of iteration |
| ---- | ---- |---- |---- |---- |---- |
| Pentium 4 3.0GHz  | 1 | 405.700	| MKL |  VASP.4.6.12 |  8 |
| Pentium D 2.8GHz  | 2 | 366.748 | ATLAS | VASP.4.6.12 |  8 |
| Pentium D 2.8GHz  | 2 | 145.897 | MKL | VASP.4.6.31| 8 |
| Athlon 4.4+GHz  | 2 | 157.976	 | ATLAS | VASP.4.6.12| 8 |
| Core2Duo 2.4GHz  | 2 |103. | MKL | VASP.4.6.12|  8 |  8 |
| Core2Quad 2.4GHz  | 4 | 107.071 | MKL | VASP.4.6.28|  8 |
| Core2Quad 2.66GHz  | 4 | 98.455 | MKL | VASP.4.6.28|   8 |
| Core2Quad 2.83Hz  | 4 | 89.891 | MKL | VASP.4.6.28|   8 |
| HA8000	情報基盤センター  | 16 | 39.550 | MKL | vasp.4.6.36|   8 |
| Core i7 3.2GHz (si1) | 4 | 45.738 | MKL | vasp.5.2.2 |   8 |
| Core i7 2600k 3.4GHz  | 4 |  38.676 | MKL | vasp.5.2.2 |   8 |
| Core i7 4770k 3.4GHz  | 4 |  18.084 | MKL | vasp.5.3.2 |   8 |
| Core i7 6770  3.4GHz  | 4 |  16.536 | MKL | vasp.5.3.2 |   8 |
| Core i7 6770  3.4GHz HT on | 8 |  18.212 | MKL | vasp.5.3.2 |   8 |
| XeonE5-2630  2.2GHz (tt30) | 20 |  14.685 | MKL | vasp.5.3.2 |   8 |
| XeonE5-2680  2.8GHz (ex1) | 20 |  8.568 | MKL | vasp.5.3.2 |   8 |
| Core i9 9940X 3.3GHz (i8) | 12 |  8.433 | MKL | vasp.6.1.2 |   8 |



# Large calculation
#### Calculatoin: Structure optimization of alpha-Al2O3 using VASP. 

| option | values |  
| ---- | ---- |
| Al2O3 supercell | Al\*48, O\*72|  
| Cutoff | 500eV |
| EDIFF | 0.0001 |
| kpt | 1x1x1 Gamma |
| EDIFFG | 0.001 |
| ISIF | 3  |
| Download .tar file | http://www.edge.iis.u-tokyo.ac.jp/vasp/speed-chk-large.tar  |

#### Results
| CPU  | # of parallel | Elapsed time (sec) | Compiler, Library, etc. |  VASP version | # of iteration |
| ---- | ---- |---- |---- |---- |---- |
| Pentium D 3.2GHz x 2  | 4 | 2289.064 | MKL | VASP.4.6.28|  11 |
| Core2Quad 2.83Hz      | 4 | 1896.565 | MKL | VASP.4.6.12|   11 |
| Core2Quad 2.83Hz x 2  | 8 | 1748.101 | MKL | VASP.4.6.35|   11 |
| Core i7 3.2GHz (si1) | 4 | 613.133 | MKL | vasp.5.2.2 |   5 |
| XeonE5-2630  2.2GHz (tt30) | 20 |  124.397  | MKL | vasp.5.3.2 |   5 |
| Core i9 7920X 2.9GHz (tt1) | 12 |   124.128 | MKL | vasp.5.4.1 |   5 |
| Core i9 9940X 3.3GHz (i9) | 12 |   150.138 | MKL | vasp.5.4.1 |   5 |
| Core i9 10920X 3.5GHz (i17) | 12 |   129.480 | MKL | vasp.6.1.2 |   5 |
| Xeon Silver4114 2.2GHz (xx1) | 20 | 62.866 | MKL | vasp.5.4.4 |   5 |
| Xeon Gold6130 2.1GHz (gx1) | 32 | 40.213 | MKL | vasp.5.4.4 |   5 |





