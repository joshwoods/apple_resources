

- Virtualization
-  Virtualize macOS on a Mac 

API Collection

# Virtualize macOS on a Mac

Configure and run macOS guests on Apple silicon.

## Overview

Use the VZVirtualMachineConfiguration to create a VZMacPlatformConfiguration that represents a specific macOS platform configuration (VZMacHardwareModel, number of virtual CPUs, RAM, devices, and so on) that you want to run on your Apple silicon Mac.

The Virtualization framework provides everything you need to macOS on a VM using macOS installation images you download from Apple. Use the latestSupported method of VZMacOSRestoreImage to obtain the URL for the installation media used to install the latest version of macOS. Alternatively, if you’ve already downloaded a macOS release, you can construct a `VZMacOSRestoreImage` object using that file. The `mostFeaturefulSupportedConfiguration` property of a `VZMacOSRestoreImage` object specifies the requirements and recommendations that you use to configure a VZVirtualMachineDelegate to complete this installation. After creating a `VZVirtualMachine`, use VZMacOSInstaller to install macOS on that virtual machine. You then use this configuration to create a bootable image that, along with a VZMacOSBootLoader, runs in a VZVirtualMachine that you can control.

For more information on running macOS as a guest, see `Creating and Running a macOS Virtual Machine`.

## Topics

### Platform components

Configure macOS guests with specific hardware capabilities and unique hardware identifiers.

class VZVirtualMachineConfiguration

The environment attributes and list of devices to use during the configuration of macOS or Linux VMs.

class VZMacOSVirtualMachineStartOptions

A class that describes start options for macOS VMs.

class VZMacPlatformConfiguration

The platform configuration for booting macOS on Apple silicon.

class VZPlatformConfiguration

The base class for a platform configuration.

class VZMacHardwareModel

A specification for the hardware elements and configurations present in a particular Mac hardware model.

class VZMacMachineIdentifier

A unique identifier for a VM.

class VZMacAuxiliaryStorage

An object that contains information the boot loader needs for booting macOS as a guest operating system.

### Boot images

Create macOS boot loaders for running macOS on Apple silicon.

class VZMacOSBootLoader

An object that loads and configures a boot loader for running macOS on Apple silicon as a guest system of your VM.

class VZBootLoader

The base class that defines the management of the initial process of the guest system.

### Installers

Create macOS installation and restoration images.

class VZMacOSInstaller

An object you use to install macOS on the specified virtual machine.

class VZMacOSRestoreImage

An object that describes a version of macOS to install on to a virtual machine.

class VZMacOSConfigurationRequirements

An object that describes the parameter constraints required by a specific configuration of macOS.

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

Virtualize Linux on a Mac

Configure and run Linux guests on Apple silicon and Intel-based Mac computers.

Running Intel Binaries in Linux VMs with Rosetta

Run x86_64 Linux binaries under ARM Linux on Apple silicon.

Accelerating the performance of Rosetta

Improve Rosetta performance by adding support for the total store ordering (TSO) memory model to your Linux kernel.

