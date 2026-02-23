# DM3730 EVK BSP

![IMG_20260223_121348](https://github.com/user-attachments/assets/c74459b9-fb51-405e-a7ff-4f4ca1bb609b)

---

## Overview

The **DM3730 EVK** is an evaluation board based on the **Texas Instruments DM3730 (OMAP3630) SoC**, a Cortex-A8 ARMv7 processor introduced in the late 2000s. 
The platform was widely used in industrial, multimedia, and embedded applications due to its:

* ARM Cortex-A8 CPU (ARMv7-A)
* NEON SIMD engine
* PowerVR SGX graphics
* GPMC (General-Purpose Memory Controller)
* Rich peripheral set (I2C, SPI, UART, MMC, USB, Ethernet, etc.)

While the hardware remains reliable and suitable for many embedded use cases, **official software support has significantly aged**. 
Most vendor repositories are outdated, tied to legacy kernels ie Linux 2.6, or depend on obsolete toolchains and build systems.

---

## Project Goal

This organization exists to provide a **clean, maintainable, and modern Board Support Package (BSP)** for the DM3730 EVK.

The goals are:

* Support modern Linux kernels
* Provide up-to-date U-Boot
* Maintain a reproducible Yocto-based build system
* Enable NFS, NAND, MMC, and Ethernet boot flows
* Maintain device tree support
* Provide long-term maintainability

Rather than relying on legacy vendor trees, this project rebuilds the software stack using modern upstream components wherever possible.

---

## Repository Structure

This organization contains:

* **Linux kernel tree** adapted for DM3730 EVK
* **U-Boot configuration** and board support
* **Yocto BSP layer (meta-dm3730)**
* Device tree sources
* Defconfigs
* Documentation and bring-up notes

Each repository is maintained independently but designed to work together as a cohesive BSP.

## Disclaimer

This is an independent community-driven effort.
It is **not affiliated with Texas Instruments or Embest**.
