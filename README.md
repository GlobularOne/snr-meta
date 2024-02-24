# Snr meta repository

Snr (Stick 'n' Run) is a project that allows generating bootable mediums based on Debian. These bootable mediums only have one purpose. To run a payload.

## Snr components

Snr is separated into several projects, which is explained in [DESIGN.md](https://github.com/GlobularOne/snr-meta/main/blob/DESIGN.md). This repository has all the snr components as submodules, so fetching all the submodules should give you the source code for all the components.

## Why generate images based on Debian to run payloads

Physical access to a device, opens many interesting opportunities. However the current methods of doing such things are either manual and time-consuming or involve sticking a usb device that has to not sound suspicious to the operating system present to function. Which is not hassle-free neither guaranteed to work. So, what if we could remove the barrier of operating system security checks, firewalls and AVs? 

And that is what snr does. Snr generates a bootable image (both BIOS and UEFI) based on Debian, as the host operating system is not even loaded, it cannot protect itself against such attacks. UEFI secure boot does no help neither, as shim is installed on the images which means whatever BIOS, UEFI, UEFI with secure boot. The payload will run.

## How to protect from such attacks 

Protection from these types of attacks is explained in [PROTECTION.md](https://github.com/GlobularOne/snr-meta/main/blob/PROTECTION.md)

## Contacting the author

You can always send an email to me. I am available as `GlobularOne@proton.me`

## Disclaimer

This project is strictly for legal and educational purposes. It hopefully helps people to take their physical security more seriously and even enhance physical penetration testing sessions. It must only be used where consent is granted to do so. We (the project development team) do not encourage or endorse any illegal activities.

## License

All of snr projects are licensed under Apache Software License 2.0. See the LICENSE file for each for more information. Documentations provided in this project (snr-meta) are released to the public space (In simpler words, do whatever you want with it) to the extent your local law allows.
