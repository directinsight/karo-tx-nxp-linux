# Build Linux for TXCOM modules based on NXP's proprietary kernel

NXP (formerly Freescale) provides access to their own git kernel repository and can be viewed at: [Public GIT](http://git.freescale.com/git/cgit.cgi/imx/linux-2.6-imx.git)

Only a few changes to the kernel sources and the description of the TXCOM module and baseboard hardware - the device tree - are needed to get it running.

The main difference between Mainline Linux and the proprietary NXP kernel are the GPU drivers. Vivante GPU drivers are only available as closed source binary blobs. Unfortunatele these are not compatible to common Linux standards but are still required for full GPU functionality. An evolving open-source alternative called Etnaviv is used for mainline Linux which might be the choice in the future.

