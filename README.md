# meta-rpi
meta layer for customized rpi image 

# Steps to Build

git clone git://git.yoctoproject.org/poky -b scarthgap 

cd poky

git clone git://git.yoctoproject.org/meta-raspberrypi -b scarthgap

git clone https://git.openembedded.org/meta-openembedded -b scarthgap

TEMPLATECONF=meta-rpi/conf/templates/default . oe-init-build-env

bitbake rpi-image

# Final Image 
will be avaiable in deploy folder

rpi-image-raspberrypi5.rootfs-XXX.wic.bz2

extarct the same and write to sd card.
