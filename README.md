# Software
Software repository of the openMRC project.

kernel - Firewire enabled Pi-5 Kernels
Scripts - Where more scripts will be added

**THE KERNELS HAVE NOT BEEN TESTED**

To install the kernels

Download all 3 .deb files. Run the following
sudo dpkg -i ../linux-image-*.deb ../linux-headers-*.deb ../linux-libc-*.deb

After it installs add the following to your config.txt

dtparam=pciex1
dtoverlay=pcie-32bit-dma

Reboot and test.