# Linux for TXCOM modules based on NXP's proprietary kernel

The main difference between Mainline Linux and the proprietary NXP kernel are the GPU drivers. Vivante GPU drivers are only available as closed source binary blobs. Unfortunatele these are not compatible to common Linux standards but are still required for full GPU functionality. An evolving open-source alternative called Etnaviv is used for mainline Linux which might be the choice in the future.

NXP (formerly Freescale) provides access to their own git kernel repository which can be viewed at: [Public GIT](http://git.freescale.com/git/cgit.cgi/imx/linux-2.6-imx.git)

Only a few changes to the kernel sources and the description of the TXCOM module and baseboard hardware - the device tree - are needed to get it running. These required steps are defined in a Yocto recipe which makes it easy to build the kernel for a Ka-Ro TXCOM.

# Build
## How to setup and use Yocto for building

The steps for building the kernel: [www.karo-electronics.com/yocto-guide](http://www.karo-electronics.com/yocto-guide)

# Device Tree 
## The description of the hardware in a system - a combination of baseboard and module
Ka-Ro Device Tree Structure for NXP Kernel in NXP Yocto BSP: [dt-karo-nxp-dt-structure.md](https://github.com/karo-electronics/documentation2/blob/master/dt-karo-nxp-dt-structure.md)
