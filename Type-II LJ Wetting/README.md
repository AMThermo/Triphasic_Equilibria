# Wetting Behavior in type-II Lennard-Jones Mixtures: A Molecular Approach
This repository contains all the LAMMPS inputs and outputs of VLLE and interfacial simulations carried out in this publication for each $\zeta$ and $\Lambda$ coordinates, as well as images of the simulation cell and specific post-processed plots for each coordinate.


### Folder Structure:
Each folder contains in its name the $\zeta$ value written after Z and the $\Lambda$ value written after L, with no floating points. Here are some examples of folder coordinates:
  - ***Z_01_L_013***: contains files for the $\zeta$=0.1 and $\Lambda$=0.13 coordinate
  - ***Z_0025_L_016***: contains files for the $\zeta$=0.025 and $\Lambda$=0.16 coordinate
    
      - ***T_1, T_2, T_3, T_4***: Folders containing LAMMPS input/output files for the MD simulations at the four temperatures reported in the publication (T_1 is the lowest and T_4 is the highest temperature).
        - ***in.lammps***: Contains the LAMMPS input file. Simulations should run only from this file.
        - ***log.lammps***: Standard output from LAMMPS containing the thermodynamic output of the system's temporal evolution.
        - ***c1.txt, c2.txt***: Density z-profiles for components 1 and 2 respectively.
        - ***tensores.txt***: Density and pressure z-profiles for the 1 + 2 mixture.
        - ***STD/***: Folder containing a time extension used to calculate the interfacial tension standard deviation. It contains its own in.lammps, log.lammps, c1.txt, c2.txt and tensores.txt files.
          
### Documents compiled in this repository:
Within each folder simulations at four different temperatures can be found. Each temperature inputs and output files are colected in each respective folder. Additionally, the following post-processing files can be found:

      
      
        
  - ***box_T_1.png, box_T_2.png, box_T_3.png, box_T_4.png***: Snapshots of the equilibrium VLLE simulation cell where grey and green spheres are components 1 and 2 respectively.
  - ***BF_lineplot***: 

### Citing this work
Please, if you use the input files or the information compiled in this page cite the original work where they come from as:
- *F.A. Figueroa, G. Alonso, A. Mejía. Wetting Behavior in type-II Lennard-Jones Mixtures: A Molecular Approach. Manuscript under preparation*
