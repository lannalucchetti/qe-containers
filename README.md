# qe-containers

to build: `sudo singularity build -F --sandbox ./sandbox/qe qe.def`

to run bash inside the container: `singularity exec ./sandbox/qe /bin/bash`

to run qe inside the container: `mpirun -np 8 singularity exec ./sandbox/qe pw.x < ./c6h6.in > qe.out &`