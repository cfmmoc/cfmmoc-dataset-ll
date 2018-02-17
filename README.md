# ![cfMMOC LOGO](https://github.com/cfmmoc/cfmmoc/blob/master/cfmmoc.png)-dataset-ll, a dataset of low-level terrains for cfMMOC demo.
Licensed under The GNU General Public License v3.0 (GPLv3)

Any modification, re-utilization or copy of the dataset in other software or publications should mention a data CITATION of this dataset.

## Overview

Hierarchical 3D models are in OGRE mesh format, and textures are in dds format. A demo using this dataset could be found at https://github.com/cfmmoc/cfmmoc.

The range of level of this dataset is from 0 (six tiles for the Globe) to 5 (6144 tiles for the Globe totally).

## Sources

The dataset is generated from Shuttle Radar Topography Mission (SRTM) v7 heightfiled dataset and Blue Marble Next Generation (BMNG) imagery dataset.

## Usage

Due to the restriction of uploading single iso large file to GitHub, massive small tile files are maintained in this repository.

Three steps for using these dataset: Cloning these data, Storing in iso image, and Mounting to http server.

1.Downloading this dataset using git:

$ git clone --depth=1 https://github.com/cfmmoc/cfmmoc-dataset-ll.git

2.Generate an iso file by using Brasero:

$ brasero -d cfmmoc-dataset-ll/sim cfmmoc-dataset-ll/com cfmmoc-dataset-ll/tex

Above command would open Brasero GUI, save it as cfmmoc-dataset-ll.iso

3.Run mount command with superuser privilege:

\# mount -o loop cfmmoc-dataset-ll.iso /var/www/html/

Finally, start httpd server with superuser privilege (make sure http server port is 80 by default):

\# service httpd start

After above configuration, REFER to this page, https://github.com/cfmmoc/cfmmoc, for compiling and runing cfMMOC demo.
