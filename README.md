# ![cfMMOC LOGO](https://github.com/cfmmoc/cfmmoc/blob/master/cfmmoc.png)-dataset-ll, a dataset of low-level terrains for cfMMOC demo.
Licensed under The GNU General Public License v3.0 (GPLv3)

Any modification, re-utilization or copy of the dataset in other software or publications should mention a data CITATION of this dataset.

## Overview

Hierarchical 3D models are in OGRE mesh format, and textures are in dds format. A demo using this dataset could be found at https://github.com/cfmmoc/cfmmoc.

The range of level of this dataset is from 0 (six tiles for the Globe) to 5 (6144 tiles for the Globe totally).

## Sources

The dataset is generated from Shuttle Radar Topography Mission (SRTM) v7 heightfiled dataset and Blue Marble Next Generation (BMNG) imagery dataset.

## Usage

Downloading this dataset using git:

$ git clone --depth=1 https://github.com/cfmmoc/cfmmoc-dataset-ll.git

Generate an iso file by using Brasero:

$ brasero 

Mount the iso file:

Start httpd server:
