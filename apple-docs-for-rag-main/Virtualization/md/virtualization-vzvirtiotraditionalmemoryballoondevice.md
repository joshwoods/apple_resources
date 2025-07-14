

- Virtualization
-  VZVirtioTraditionalMemoryBalloonDevice 

Class

# VZVirtioTraditionalMemoryBalloonDevice

The object you use to change the amount of memory allocated to the guest system.

macOS 11.0+

``` source
class VZVirtioTraditionalMemoryBalloonDevice
```

## Overview

A VZVirtioTraditionalMemoryBalloonDevice object implements a Virtio-compliant balloon memory device, which lets you change the amount of physical memory assigned to the guest operating system. The virtual machine has no insight into the amount of memory its guest operating system uses. A memory balloon device lets you ask the guest operating system to relinquish memory voluntarily, which you might do if memory resources become scarce.

You don’t create a VZVirtioTraditionalMemoryBalloonDevice object directly. Instead, create a VZVirtioTraditionalMemoryBalloonDeviceConfiguration object and assign it to the memoryBalloonDevices property of your virtual machine configuration. In response, the virtual machine creates this object and assigns it to its memoryBalloonDevices property.

To use a memory balloon device, change the value in the targetVirtualMachineMemorySize property when your virtual machine is running. If the new value is smaller than the amount of currently assigned memory, the guest system may return a list of unused memory pages using the memory balloon device. If it does, the virtual machine releases those pages back to the host computer. If it doesn’t return any memory pages, the virtual machine leaves the guest’s memory size unchanged. If the new value is larger than the amount of currently assigned memory, the virtual machine reserves more pages for the guest operating system.

For optimal performance, the guest operating system should compact its memory before returning any pages back to the memory balloon device. Compacting the memory reduces fragmentation, and allows it to return contiguous blocks of free pages in the memory balloon device.

## Topics

### Changing the memory partition size

var targetVirtualMachineMemorySize: UInt64

The target amount of memory, in bytes, to make available to the virtual machine.

## Relationships

### Inherits From

- VZMemoryBalloonDevice

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Memory balloon devices

class VZMemoryBalloonDevice

The common behavior for memory devices.

