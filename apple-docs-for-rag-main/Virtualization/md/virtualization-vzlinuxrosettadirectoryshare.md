

- Virtualization
-  VZLinuxRosettaDirectoryShare 

Class

# VZLinuxRosettaDirectoryShare

The Linux directory share for Rosetta.

macOS 13.0+

``` source
class VZLinuxRosettaDirectoryShare
```

## Overview

This directory share exposes the Rosetta directory from the host file system to the guest. The example below shows the process of creating a VZVirtualMachineConfiguration, and then associating the Rosetta directory share with the VM configuration.

```
let tag = "EXAMPLE_TAG"  
let configuration = VZVirtualMachineConfiguration()
do {
    try let validationError = VZVirtioFileSystemDeviceConfiguration.validateTag(tag)
    let rosettaDirectoryShare = try VZLinuxRosettaDirectoryShare()
    let fileSystemDevice = VZVirtioFileSystemDeviceConfiguration(tag: tag)
    fileSystemDevice.share = rosettaDirectoryShare

    configuration.directorySharingDevices = [ fileSystemDevice ]
} catch VZError.invalidVirtualMachineConfiguration {
    // Rosetta is unavailable.
}
```

For complete instructions on installing Rosetta see Running Intel Binaries in Linux VMs with Rosetta, which includes additional information about checking for Rosetta availability, mounting the directory share, and registering the Rosetta runtime binary to run Intel binaries in a guest VM.

For information on using a custom kernel to enhance Rosetta performance, see Accelerating the performance of Rosetta.

## Topics

### Creating a Rosetta directory share

init() throws

Creates a new Rosetta directory share, or returns an error if Rosetta isn’t installed.

### Checking Rosetta availability

class var availability: VZLinuxRosettaAvailability

A value that indicates the current state of Rosetta’s availability.

enum VZLinuxRosettaAvailability

Constants that describe the availability and installation status of Rosetta.

### Installing Rosetta

class func installRosetta(completionHandler: ((any Error)?) -> Void)

Starts the installation of Rosetta.

### Setting the ahead of time (AOT) caching options

var cachingOptions: VZLinuxRosettaDirectoryShare.CachingOptions?

The value that enables translation caching and configures the socket communication type for Rosetta.

func setCachingOptions(VZLinuxRosettaDirectoryShare.CachingOptions?) throws

Sets the Rosetta caching options using the options you specify.

enum CachingOptions

Socket values you specify to configure Rosetta’s caching capabilities.

## Relationships

### Inherits From

- VZDirectoryShare

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Related Documentation

class VZDirectorySharingDeviceConfiguration

The base class for a directory sharing device configuration.

class VZSharedDirectory

A directory on the host that you can expose to a guest.

class VZSingleDirectoryShare

An object that defines the directory share for a single directory.

class VZMultipleDirectoryShare

An object that describes a directory share for multiple directories.

### Runtime

class VZVirtualMachine

An object that manages the overall state and configuration of your VM.

class VZVirtualMachineView

A view that allows user interaction with a VM.

