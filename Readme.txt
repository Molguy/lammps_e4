Ejemplo 4. Equilibrio L-V para un sistema Lennard-Jones

En la carpeta debe haber:
 a) inLV.lj

1. Abrir el archivo inLV.lj para analizarlo, la temperatura es 0.7.

2. Ejecutar la simulación usando:
   ./lmp_mpi < inLV_0.7.lj

3. Visualizar el comportamiento final del archivo de salida dump.nvt con Ovito
   ovito dump_0.7.nvt

4. Efectuar la gráfica del perfil de densidad usando:
   tail -504 densityprofx_0.7.out > denx_0.7.out
   xmgrace -block denx_0.7.out -bxy 2:4

5. Ver el perfil de temperatura usando:
   xmgrace tei_0.7.out

6. Ver el perfil de la componente yz del tensor de presión (Pyz)
   xmgrace prico_0.7.out

Cambiar la temperatura a 1.0 y repite el análisis.
