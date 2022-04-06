
# My stealth QEMU build for hide your presence

## Whats this ? 
This repository contains a git snapshot version of QEMU with KVM stealth patches applied to fool programs that look for signs of VirtualBox, Virtual PC, Bochs, QEMU/KVM and VMWare.

By using this QEMU, you can hide your presence from anti-cheat vendors.

## Precautions

-   **Under no circumstances** should you run this stealth-patched version of QEMU as a daily driver. The code is from the official Git repository and could be in whatever state. While I have successfully booted a Windows 10 (20H2) virtual machine and it works for me, it may not work as intended for you. You've been warned.
-   This version of QEMU is also great for debugging anti-tamper/anti-VM mechanisms in software or analysing suspicious software that are hostile to VM environments.
-   Do **not** simply run `make install` once you've built QEMU! You will most likely overwrite your virgin QEMU that was supplied either by compiling an official QEMU release or using a package supplied by your distro repositories. I'd honestly recommend copying the built binary to the folder you have your work directory prepared in and run it from there.
