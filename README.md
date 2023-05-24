# Sea-Fans
Python and LAMMPS code for 3D Molecular Dynamics Simulations, starting from 2D photos of network and tree sea fans.

Sea fans are a variety of corals structured in a flat fanlike pattern of numerous cylindrical polyps. Their morphology has been previously studied through 2D images and digitized data points depicting the structures have been obtained. The project employs polymer physics and molecular simulations to study samples of tree-like and network structures and analyze differences in their dynamics. The sea fans’ motion was simulated with the Large-scale Atomic/Molecular Massively Parallel Simulator Molecular Dynamics software by connecting the data points through harmonic bonds and modulating the flexibility/bending stiffness through an angle potential between three particles. Preliminary analysis of the output through particle displacements computations suggests that tree structures tend to be more dynamic than networks and that the greatest displacements correspond to outer particles, a result consistent with experimental findings. Further analysis of all available structures is necessary to conclusively find the correlation between the morphology of sea fans and their environment. 

Tree_Input.txt is the data file containing the 3D positions of all the tree (branched) sea fan atoms, bonds, and angles created. 

Network_Input.txt is the data file containing the 3D positions of all the network (mesh) sea fan atoms, bonds, and angles created. 

Equilibration_Code.txt is the Python file that outputs the file used by LAMMPS for the initial equilibration simulation. It also checks whether the equilibration worked or not after it is run. 

LAMMPS_Equilibration_Input.txt is the data file read by LAMMPS to create the initial equilibration simulation. 

LAMMPS_Input.txt is the data file read by LAMMPS to create the dynamics simulations and the nutrients capture simulations.

Displacements_Calculations_Code.txt is the Python file that contains the analysis (plotting MSD, maximum displacement per particle, average displacement for the most dynamics atoms) done on the output of the simulations. 

Nutrients_Capture_Code.txt is the Python file that calculates the number of nutrients captured by the sea fan at each timestep.
