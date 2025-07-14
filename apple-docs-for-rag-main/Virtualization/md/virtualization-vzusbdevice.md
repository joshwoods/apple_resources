

- Virtualization
-  VZUSBDevice 

Protocol

# VZUSBDevice

A protocol that represents a USB device in a VM.

macOS 15.0+

``` source
protocol VZUSBDevice : NSObjectProtocol
```

## Overview

Classes that conform to this protocol represent hot-pluggable USB devices.

Important

Don’t use the `VZUSBDevice` protocol with objects outside the Virtualization framework. This protocol only describes capabilities of Virtualization framework objects.

## Topics

### Properties

var usbController: VZUSBController?

The USB controller that has an attachment to the device.

**Required**

var uuid: UUID

The device’s unique identifier.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- VZUSBMassStorageDevice

## See Also

### Related Documentation

class VZUSBMassStorageDevice

A class that represents a hot-pluggable USB mass storage device.

### Protocols

protocol VZUSBDeviceConfiguration

The protocol for configuring USB devices.

