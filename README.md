# coreinit

## About

<div style="display: flex;">
  <img src="splash.png" width="200" />
  <img src="bootmenu.png" width="200" />
  <img src="firmware-setup.png" width="200" />
</div><br>

coreinit is a modular, minimal bootloader. It aims to provide a clean, extensible startup experience for your operating systems. Written in Turbowarp, it handles system initiation and provides the boot splash and optionally, boot menu and firmware setup.<br>

> *Starting from release 1.3, coreinit will be Turbowarp-exclusive, and will not work in Scratch. For release 1.2 and below, coreinit-firmware-setup is Turbowarp-exclusive. All other sprites work in Scratch.*

coreinit-bootmenu handles the boot menu for coreinit. It allows you to select different operating systems to boot and access the firmware setup utility. coreinit works just fine without coreinit-bootmenu, and coreinit-bootmenu works just fine without coreinit (although it will not initialize without the "coreinit-initialize" message).

coreinit-firmware-setup is the utility which allows you to modify the Scratch runtime. It is extremely powerful, allowing you to change the clone limit, your username, framerate limit, stage resolution, and more. coreinit-firmware-setup requires coreinit-bootmenu for it to be accessed.

coreinit-updater is the utility which allows you to update coreinit with a click of a button. Internet connection required. coreinit-updater requires coreinit-bootmenu for it to be accessed.

## Features

coreinit features:
- Extremely modular, with everything being optional
- Easily customizable with barely any branding
- Modifiable with easy-to-read code
- Faster and easier than coding your own boot splash

## Installation

Simply import the "coreinit" sprite into your project. Remember to make all your scripts start after the "coreboot_boot" message and end after the "coreboot_shutdown" message. For no layering problems, you should hide all sprites before "coreboot_boot" and after "coreboot_shutdown". Optionally, you can also import the "coreinit-bootmenu" and "coreinit-firmware-setup" sprites for a more complete experience.
