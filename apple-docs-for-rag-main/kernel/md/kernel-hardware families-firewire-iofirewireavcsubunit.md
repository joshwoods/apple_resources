

- Kernel
- Hardware Families
- FireWire
-  IOFireWireAVCSubUnit 

Class

# IOFireWireAVCSubUnit

nub for sub unit of AVC devices. Just for matching, calls the AVC unit for all functions.

macOS 10.2+

``` source
class IOFireWireAVCSubUnit : IOFireWireAVCNub
```

## Overview

## Topics

### Miscellaneous

AVCCommand

Sends an AVC command to the device and stores the response.

AVCCommandInGeneration

Sends an AVC command to the device and stores the response. The command must complete in the specified FireWire bus generation otherwise kIOFireWireBusReset is returned.

handleClose

Overrideable method to control the open / close behaviour of an IOService.

handleOpen

Overrideable method to control the open / close behaviour of an IOService.

matchPropertyTable

Matching language support Match on the following properties of the sub unit: Vendor_ID GUID SubUnit_Type

updateAVCCommandTimeout

By default, AVCCommands timeout 10 seconds after receiving an Interim response. This function resets the timeout of the current command to 10 seconds from the current time. Call this repeatedly for AVC commands that take a very long time to execute to prevent premature timeout.

### DataTypes

ExpansionData

### Instance Variables

reserved

### Instance Methods

- AVCCommand

- AVCCommandInGeneration

- getMetaClass

- handleClose

- handleOpen

- init

- matchPropertyTable

- message

- updateAVCCommandTimeout

## Relationships

### Inherits From

- IOFireWireAVCNub

## See Also

### Nubs

IOFireWireLocalNode

IOFireWireSBP2LUN

Provider for most drivers.

IOFireWireAVCUnit

nub for AVC devices

IOFireWireAVCNub

nub for AVC devices

IOFireWireUnit

IOFireWireNub

