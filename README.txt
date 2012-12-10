>>>PROGRAM TITLE
ALCBEAM


>>>>LICENCE AGREEMENT (9 Dec 2012)
ALCBEAM development is funded by the US Department of Energy (DoE), and distribution is subject to DoE requirements and restrictions.

In order to acquire access to the code sources, the recipient agrees:

1) to use the ALCBEAM source code AS IS without modification; users however are welcome to request changes, or to contribute modifications subject to approval of the authors;
2) if the copy of the ALCBEAM downloaded by the authorized user is made available to third parties, to ensure that the user agreement is followed by the third parties;
3) to inform the first author of the code of planned research using that module;
4) prior to publication, to communicate any significant results derived from a module to the main author;
5) to include in any published results, talks or presentations the proper code name(s) and appropriate reference. 


>>>INTRODUCTION
ALCBEAM is a three-dimensional neutral beam formation and propagation code. It is developed as a supplemental tool for beam-based plasma diagnostics at Alcator C-Mod tokamak.
It can be used for simulation of the neutral beams used on other tokamaks, stellarators or other magnetic fusion devices.
The code effectively unifies the beam formation and extraction processes with beam attenuation and excitation in plasma and residual gas in the beam duct. 
The goal of the code is to provide reliable estimates of the local beam equilibrium parameters: such as beam energy fractions, density profiles and excitation populations.
The extraction model uses the semi-empirical description to simulate the processes in the beam ion source which effect the beam formation.


>>>OPERATING SYSTEM
Linux

>>>PROGRAMMING LANGUAGE
IDL


>>>FILES
1) alcbeam.pro - main IDL code.
2) adas - directory contains the ADAS format data files to be used by alcbeam.pro
3) alcbeam_manual.pef - most recent manual in pdf format.
4) DNBI_TEST.abi - sample input data file
5) DNBI_TEST.abo - sample output data file
 

>>>INITIALIZATION
1) CD to the directory where alcbeam.pro is located 
example ($ cd /home/$USER/alcbeam/)
2) Open a new IDL session:
$ idl
3) Compile the code:
IDL> .r alcbeam.pro
4) Run the ALCBEAM procedure:
IDL> alcbeam
5) Wait for GUI to initialize. Wait for status message:
:->>> Initializing …
1 : [date] Ready !!!


>>>TO READ AND PREVIEW TEST OUTPUT DATA
1) Chage the path in the test box (under the 'Read/View Results from Previous Runs") to the directory, where DNBI_TEST.abo file is located.
2) Hit the "Search Available Runs" button.
3) Select DNBI_TEST.abo in the box to the right.
4) Hit "Read Results" button. Output data is extracted from the file and is ready for preview.
5) Use the 'Plot" button on the bottom/middle of the alcbeam GUI to plot the output data.
6) All the plots can be exported into png image or ascii-text files.


>>>TO PERFROM A TEST RUN
1) HIT "PREPARE A RUN" button.
2) HIT "Settings" button (to the right from LOAD button). A new window is opened.
3) Select 'Load all data from "*.abi input file".
4) Make sure that all paths to the DNBI_TEST.abi file are correct.
5) HIT "Save" button.
6) Hit 'Close" button.
7) Hit 'Load" button. All input data is loaded from DNBI_TEST.abi file. LOAD panel is dimmed.
8) Hit "Settings" button (to the right from CONSTRUCT button). A new window is opened.
9) Change PATH in "Location of ADAS files" to the adas directory.
10) HIT "Save" button.
11) Hit 'Close" button.
12) Hit 'CONSTRUCT" button. All 3D arrays are constructed from inpur data. CONSTRUCT panel is dimmed.
13) Hit "Settings" button (to the right from CALC button). A new window is opened.
14) Change "Save output to" "*.abo output file". Select name for any new *.abo file, where data is to be saved.
15) HIT "Save" button.
16) Hit 'Close" button.
17) Hit "CALC" button.
18) The calculation is started. The progress is shown in the status window. Running time for test run is 5-15 minutes.
19) Once the calculation is finished the output data is saved into the *.abo file.
20) Use the 'Plot" button to plot the output data.
21) All the plots can be exported into png image or ascii-text files.











