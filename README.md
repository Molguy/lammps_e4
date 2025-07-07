# lammps_e4

Instructivo, archivos de entrada y log's de la simulación del ejemplo 4,

para la temperatura de 0.7:

    mpirun -np 4 lmp_mpi < inLV_0.7.lj
. 

    ovito < dump_0.7.nvt
.

    tail -504 densityprofx_0.7.out | xmgrace -block - -bxy 2:4
.

    xmgrace tei_0.7.out && xmgrace prico_0.7.out
.
para la temperatura de 1.0:

    mpirun -np 4 lmp_mpi < inLV_1.0.lj
. 

    ovito < dump_1.nvt
.

    tail -504 densityprofx_1.out | xmgrace -block - -bxy 2:4
.

    xmgrace temperatura_1.out && xmgrace prico_1.out
