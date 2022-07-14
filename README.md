# PySEBS <img src="readme/PySEBS.png" align="right" height="15%" width="15%"/>

The `PySEBS` is a software that can be used to calculate actual evapotranspiration (ETa) on a spatial scale based on the Surface Energy Balance System model (SEBS). The software is written in `Python 2.7.14` due to Python (2.7) being the latest version supported by `ArcGIS 10.1-10.6`. 

## Installing the PySEBS and software requirements

Since ETa is calculated on a spatial scale, the software operation utilizes some of the built-in tools in ArcGIS and the proper operation of these tools depends on calling of the Arcpy package in ArcGIS. Therefore, the user needs to ensure that the ArcGIS software is installed successfully. 

The PySEBS software is compressed into a `PySEBS V1.0.0.zip` file. The schematic diagram of `PySEBS file structure` is shown in the following figure. The schematic box labeled ./PySEBS/ represents a folder named `PySEBS` in the working directory, where the `PySEBS 1.0.0.zip` file will be stored after extraction. The PySEBS folder contains two parts: the `PySEBS V1.0.0.exe` program; and the `site-packages` folder containing the code libraries (arcpy package, numpy package, pandas package, Pyshp package, etc.) and the configuration Desktop.pth file.


<img src="readme/PySEBS software file structure.jpg" height="90%" width="90%" style="display: block; margin: auto;"/>

To successfully run the software, the file path of the bin folder in the ArcGIS installation directory must be added to the `Desktop.pth` file so that the arcpy packages can be properly called (see th following figure for the procedure). The path of the bin folder in the ArcGIS installation directory is usually: `.\ArcGIS\Desktop10.6\bin`; and the location of the Desktop.pth file is: `.\PySEBS\site-packages`.

<img src="readme/Add the bin folder to the Desktop.pth.jpg" height="80%" width="80%"/>


## Graphical User Interface Introduction

`PySEBS` software is a concise and straightforward scientific computing tool. It contains one main interface and three sub-interfaces . The main interface consists of three button controls: the `remote sensing data processing module` button, the `meteorological data processing module` button, and the `PySEBS calculation and processing module` button. Each button control accesses the corresponding module (sub-interface): `Module 1 - Remote Sensing Data Processing interface`, `Module 2 - Meteorological Data Processing interface`, and `Module 3 - PySEBS Calculation Procedure interface`.

<img src="readme/PySEBS GUI.jpg" />


