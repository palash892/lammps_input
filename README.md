### 🧾 LAMMPS Input Files

This folder contains input scripts for running molecular dynamics simulations using LAMMPS.

#### Files:

- **`org_equilibriate.run`**  
  Script used to equilibrate the system before the production run.

- **`ssproduction.run`**  
  Script for carrying out the production simulation after equilibration.

- **`in.production`**  
  A helper input file that serves as documentation. It contains detailed comments explaining various commonly used lines in a typical LAMMPS input file, useful for customization or reference.

### 🚀 How to Run LAMMPS Using MPI

You can run a LAMMPS input file in parallel using `mpirun` as follows:

```bash
mpirun -np <num_processors> lmp_mpi -in <input_file>
mpirun -np 8 lmp_mpi -in org_equilibriate.run
