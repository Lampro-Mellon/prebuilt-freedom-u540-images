# prebuilt-hfu-images

This repository is maintained by Software Development team at Lampro Mellon, who:

- Develop linux device drivers for RISC V based boards
- Develop applications for RISC V platforms

The repository contains prebuilt images for HiFive Unleashed board. All the linux images are built by employing, openembedded based, Freedom-U-SDK provided by SiFive.

# Directory Structure
Following is the description of directories in this repo:

**cli/**: Command Line Interface image.

**xfce4**: GUI based image for HiFive Unleashed + Expansion board.

**cli-debug**: Command Line Interface image with debug packages.

**opencv**: CLI based image with Python packages added. For details of packages, see *opencv/README.md*

# Flashing the Images

All the images can be flashed to uSD card using *bmaptool* utility. Steps are as follows:

1- Download both images (\*.wic.gz as well as \*wic.bmap)

2- Insert the card in PC and check device file /dev/sdX.

3- run *bmaptool copy demo-coreip-XYZ.wic.gz /dev/sdX*

3- Insert the card into the target.

4- Login is **root**, Password is **sifive**
