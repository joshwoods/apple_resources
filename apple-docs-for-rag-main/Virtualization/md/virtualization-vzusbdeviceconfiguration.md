

- Virtualization
-  VZUSBDeviceConfiguration 

Protocol

# VZUSBDeviceConfiguration

The protocol for configuring USB devices.

macOS 15.0+

``` source
protocol VZUSBDeviceConfiguration : NSObjectProtocol
```

## Overview

Classes that conform to this protocol represent hot-pluggable USB device configurations.

Important

Don’t use the `VZUSBDeviceConfiguration` protocol with objects outside the Virtualization framework. This protocol only describes capabilities of Virtualization framework objects.

## Topics

### Properties

var uuid: UUID

The device’s unique identifier.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- VZUSBMassStorageDeviceConfiguration

## See Also

### Protocols

protocol VZUSBDevice

A protocol that represents a USB device in a VM.

