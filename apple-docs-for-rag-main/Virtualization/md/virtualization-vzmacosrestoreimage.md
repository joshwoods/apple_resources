

- Virtualization
-  VZMacOSRestoreImage 

Class

# VZMacOSRestoreImage

An object that describes a version of macOS to install on to a virtual machine.

macOS 12.0+

``` source
class VZMacOSRestoreImage
```

## Mentioned in 

Installing macOS on a Virtual Machine

Using iCloud with macOS virtual machines

## Overview

To set up a new VM compatible with the restore image, use mostFeaturefulSupportedConfiguration to obtain the hardwareModel of the VZMacPlatformConfiguration. Then, create a VZMacOSRestoreImage object by loading an installation media file. Initialize a VZMacOSInstaller object with this `VZMacOSRestoreImage` object to install the operating system onto a VM.

Important

Loading a restore image requires the app to have the com.apple.security.virtualization entitlement.

## Topics

### Getting Information About the Restore Image

var buildVersion: String

The build version this restore image contains.

var isSupported: Bool

A Boolean value that indicates whether the current host supports this restore image.

var mostFeaturefulSupportedConfiguration: VZMacOSConfigurationRequirements?

This object represents the most fully featured configuration that’s supported by both the current host and by this restore image.

var operatingSystemVersion: OperatingSystemVersion

The operating system version this restore image contains.

var url: URL

The URL of this restore image.

### Controlling the Restoration Process

class func fetchLatestSupported(completionHandler: (Result&lt;VZMacOSRestoreImage, any Error>) -> Void)

Fetches the latest restore image supported by this host from the network.

class func load(from: URL, completionHandler: (Result&lt;VZMacOSRestoreImage, any Error>) -> Void)

Load a restore image from a file on the local file system.

class var latestSupported: VZMacOSRestoreImage

Fetches the latest restore image supported by this host from the network.

class func image(from: URL) async throws -> VZMacOSRestoreImage

Load a restore image from a file on the local file system.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Related Documentation

class VZMacHardwareModel

A specification for the hardware elements and configurations present in a particular Mac hardware model.

### Installers

class VZMacOSInstaller

An object you use to install macOS on the specified virtual machine.

class VZMacOSConfigurationRequirements

An object that describes the parameter constraints required by a specific configuration of macOS.

