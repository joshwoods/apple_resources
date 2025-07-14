

- Virtualization
-  Virtualize Linux on a Mac 

API Collection

# Virtualize Linux on a Mac

Configure and run Linux guests on Apple silicon and Intel-based Mac computers.

## Overview

Use VZVirtualMachineConfiguration to create a configuration that represents a specific Linux platform with the devices you want to use with your virtual machine (VM) — like VZVirtioSoundDeviceConfiguration or VZUSBKeyboardConfiguration.

You use this configuration to load a Linux kernel image from disk that — using VZLinuxBootLoader — runs in a VZVirtualMachine that you control.

For more information about running a Linux guest, including how to download kernel and RAM disk images, see Creating and Running a Linux Virtual Machine. For more information about running GUI Linux virtual machines, see Running GUI Linux in a virtual machine on a Mac.

## Topics

### Configurations

class VZVirtualMachineConfiguration

The environment attributes and list of devices to use during the configuration of macOS or Linux VMs.

class VZVirtualMachineStartOptions

The abstract class for VM start options.

class VZGenericPlatformConfiguration

The platform configuration for a generic Intel or ARM virtual machine.

class VZPlatformConfiguration

The base class for a platform configuration.

### Boot loaders

class VZBootLoader

The base class that defines the management of the initial process of the guest system.

class VZLinuxBootLoader

An object that loads and configures a Linux kernel as the guest system of your VM.

class VZEFIBootLoader

The boot loader configuration the system uses to boot guest-operating systems that expect an Extensible Firmware Interface (EFI) ROM.

class VZEFIVariableStore

An object that represents the Extensible Firmware Interface (EFI) variable store that contains NVRAM variables the EFI exposes.

## See Also

### Virtual machine setup

Running macOS in a virtual machine on Apple silicon

Install and run macOS in a virtual machine using the Virtualization framework.

Running Linux in a Virtual Machine

Run a Linux operating system on your Mac using the Virtualization framework.

Running GUI Linux in a virtual machine on a Mac

Install and run GUI Linux in a virtual machine using the Virtualization framework.

Installing macOS on a Virtual Machine

Download a macOS restore image and install it in a new VM.

Creating and Running a Linux Virtual Machine

Design and run custom Linux guests on Apple silicon or Intel-based Mac Computers.

Virtualize macOS on a Mac

Configure and run macOS guests on Apple silicon.

Running Intel Binaries in Linux VMs with Rosetta

Run x86_64 Linux binaries under ARM Linux on Apple silicon.

Accelerating the performance of Rosetta

Improve Rosetta performance by adding support for the total store ordering (TSO) memory model to your Linux kernel.

