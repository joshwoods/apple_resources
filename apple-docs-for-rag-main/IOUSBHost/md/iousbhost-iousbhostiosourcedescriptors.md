

- IOUSBHost
-  IOUSBHostIOSourceDescriptors 

Structure

# IOUSBHostIOSourceDescriptors

The descriptors for a single endpoint.

Mac Catalyst 14.0+macOS 10.15+

``` source
struct IOUSBHostIOSourceDescriptors
```

## Overview

The IOUSBHostIOSourceDescriptors structure initializes and adjusts pipes in the system.

## Topics

### Descriptors

var bcdUSB: UInt16

The USB version that the device supports.

var descriptor: IOUSBEndpointDescriptor

The descriptor for a USB endpoint.

var ssCompanionDescriptor: IOUSBSuperSpeedEndpointCompanionDescriptor

The descriptor for a SuperSpeed USB endpoint companion.

var sspCompanionDescriptor: IOUSBSuperSpeedPlusIsochronousEndpointCompanionDescriptor

The descriptor for a SuperSpeedPlus isochronous USB endpoint companion.

### Initializing the Structure

init()

Creates a new source descriptor structure.

init(bcdUSB: UInt16, descriptor: IOUSBEndpointDescriptor, ssCompanionDescriptor: IOUSBSuperSpeedEndpointCompanionDescriptor, sspCompanionDescriptor: IOUSBSuperSpeedPlusIsochronousEndpointCompanionDescriptor)

Creates a new source descriptor structure.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Managing Periodic Bandwidth

func adjust(with: UnsafePointer&lt;IOUSBHostIOSourceDescriptors>) throws

Adjusts the behavior of periodic endpoints to consume a different amount of bus bandwidth.

var descriptors: UnsafePointer&lt;IOUSBHostIOSourceDescriptors>

A property that retrieves the current endpoint descriptors controlling the endpoint.

var originalDescriptors: UnsafePointer&lt;IOUSBHostIOSourceDescriptors>

A property that retrieves the original endpoint descriptors from the pipe at the point of creation.

