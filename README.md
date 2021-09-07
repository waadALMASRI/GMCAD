# GMCAD: Geometric Mechanical CAD dataset

## Introduction
GMCAD is a dataset containing 2D truss-like designs along their mechanical and geometrical constraints.

The designs can be found in their CAD-like format (as .vtk), which can be viewed using [ParaView](https://www.paraview.org/download/) and their image-like format (as .png).
The 2D designs were created via [Pygmsh](https://pygmsh.readthedocs.io/en/latest/), a python library to draw CADs.
With pygmsh, every design is a combination of beams (a beam is a rectangular element), such that we save the coordinates of the 4 points of this beam. 

The mechanical conditions are:
- The Boundary conditions
- The loads
- The volume fraction (percentage of material)

The geometrical conditions that we extracted from the CAD:
- The min/max beam-width 
- The min/max beam-length
- The min overang: the overhang is the angle between the normal of the beam and the build direction (the build direction here in 2D is considered the y-axis direction)
- The total number of beams

GMCAD's inception is detailed in the article "GMCAD: an original Synthetic Dataset of 2D Designs along their Geometrical and Mechanical Conditions" accepted to the conference [ISM 2021](http://www.msc-les.org/ism2021/).

## Content of GMCAD
GMCAD's repository consists of 3 main elements:
- The CAD file: it contains the designs in .vtk format
- The image file: it contains the designs in .png format
- The parameters file: it contains the mechanical and geometrical constraints of the designs

## Link to download GMCAD
The link to download GMCAD is: https://drive.google.com/file/d/1fNnuKPTVygAM3UQgdeFdi9CJtvKGaCGG/view?usp=sharing and https://drive.google.com/file/d/1yRSBJhvPiOuNwdnbbIEqZepAjNNwYqiR/view?usp=sharing

## How to use GMCAD?
The jupyter notebook Explore_GMCAD.ipynb explains in details how to read and explore GMCAD.
