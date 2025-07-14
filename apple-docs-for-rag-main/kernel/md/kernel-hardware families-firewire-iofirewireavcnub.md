

- Kernel
- Hardware Families
- FireWire
-  IOFireWireAVCNub 

Class

# IOFireWireAVCNub

nub for AVC devices

macOS 10.2+

``` source
class IOFireWireAVCNub : IOService
```

## Overview

## Topics

### Miscellaneous

AVCCommand

Sends an AVC command to the device and stores the response.

AVCCommandInGeneration

Sends an AVC command to the device and stores the response. The command must complete in the specified FireWire bus generation otherwise kIOFireWireBusReset is returned.

getDevice

Returns the FireWire device nub that is this object's provider .

updateAVCCommandTimeout

By default, AVCCommands timeout 10 seconds after receiving an Interim response. This function resets the timeout of the current command to 10 seconds from the current time. Call this repeatedly for AVC commands that take a very long time to execute to prevent premature timeout.

### Instance Methods

- AVCCommand

- AVCCommandInGeneration

- getDevice

- getMetaClass

- updateAVCCommandTimeout

## Relationships

### Inherits From

- IOService

## See Also

### Nubs

IOFireWireLocalNode

IOFireWireSBP2LUN

Provider for most drivers.

IOFireWireAVCSubUnit

nub for sub unit of AVC devices. Just for matching, calls the AVC unit for all functions.

IOFireWireAVCUnit

nub for AVC devices

IOFireWireUnit

IOFireWireNub

