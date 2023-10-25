# NixOS-Config
This Project holds the current NixOS system configuration for all the systems that I own.

This will make updating all my systems with specific prefences and tools from a central place easy.

**Note**: This is presently under active development while I study the Nix echosystem and the file structure will change significantly during this process.

# Current Obectives

1. Create a basic NixOS system config for different systems (`Virtualbox VM` and  `Lenovo X230 Laptop`) that has the following basic configurations:
  * [ ] Systemd bootloader (EFI)
  * [ ] Luks Encrypted partitions (different passwords) - Challenge: How to secure these passwords (from this public repo) while making them available to NixOS to build with.  
  * [ ] Loading screens - Challenge: How to dynamically select loading screen based on system
  * [ ] Hardware Specific - Challenge: Dynamically select the hardware configs while avoiding `nixos-generate-config` from overriding the config.


2. Create a basic Nixpkgs manager config that can be used on existing operating systems to manage tool chains and configs that can be used on both Manjaro and MacOS.
   * [ ] Create a work profile that can be used to manage commandline tools for work
   * [ ] Replicate this work environment on the Manjaro system
   * [ ] Then extend the work profile and sync it back to the MacOS laptop
