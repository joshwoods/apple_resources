

- Virtualization
-  Virtualization enumerations 

API Collection

# Virtualization enumerations

Control the caching modes, disk synchronization, and macOS auxiliary storage options of VMs.

## Overview

These are values you use to control aspects of the operation of the virtual drives for guest VMs and the auxiliary storage of macOS guest VMs.

## Topics

### Virtual disk image caching modes

enum VZDiskImageCachingMode

An integer that describes the disk image caching mode.

### Virtual disk synchronization modes

enum VZDiskImageSynchronizationMode

An integer that describes the disk image synchronization mode.

enum VZDiskSynchronizationMode

Values that describe the synchronization modes available to the guest OS.

### Mac-specific auxiliary storage options

struct InitializationOptions

Options you can set when creating new auxiliary storage.

### Rosetta availability states

enum VZLinuxRosettaAvailability

Constants that describe the availability and installation status of Rosetta.

### Virtualization error codes

enum Code

Errors you might encounter when configuring or using a virtual machine.

### VM states

enum State

The execution states of the VM.

