# GeoMPMGen GUI Installer


This repository hosts the GUI installer for the paper: **"A 3D Material Point Discretization Approach for Complex Terrain and Geological Body: Numerical Implementation and Application."** 

The program supports Windows 10/11 platforms and includes examples demonstrated in the paper.

![Example Image](img\readme.png)

## Features

1. Supports creation of geotechnical models.
2. Includes example files for easy setup.
3. Outputs models for visualization in ParaView.

## Installation
Download and run the GeoMPMGen.exe installer.
Follow the on-screen instructions to complete the installation.

## Usage
1. Launch the application by clicking GeoMPMGen.exe.

2. You can create a geotechnical model using mesh processing software and add it to the program by selecting Add Files.Alternatively, load an example directly by using Load Params to select JSON files from the example folder.

3. Choose the output paths for the model and VTK files.
Set the generation parameters as needed.
Click Generate to create the model.

4. Visualization: Once generated, use **ParaView** to visualize the output vtu models. In addition, the model is written as ASCII, using python **numpy** to load and change the model as you like:

~~~ python
np.loadtxt('path\\to\\your\\model.mpm',delimiter=' ',skiprows=3)
~~~

**Important Note**: If the output path is on the C: drive, you must run the program as an administrator to ensure successful output generation. Failure to do so will result in no output files being created.

## Support

For any issues or questions, please open an issue in this repository.

Thank you for using GeoMPMGen!