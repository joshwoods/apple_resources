

- Kernel
- Hardware Families
- ATA
-  ATADeviceNub 

Class

# ATADeviceNub

ATADeviceNub is a concrete implementation of IOATADevice.

macOS 11.0+

``` source
class ATADeviceNub : IOATADevice
```

## Overview

clients of IOATA (disk drivers) should use the interface presented by IOATADevice. Concrete nubs are private to the IOATA family and specific subclasses of IOATADevice are instantiated by controller drivers to provide the abstract interface to clients.

## Topics

### Miscellaneous

allocCommand

create command objects for clients.

ataDeviceNub

static creator function - used by IOATAControllers to create nubs.

attach

override of IOService method.

executeCommand

Submit IO requests

freeCommand

Clients use this method to dispose of command objects.

getDeviceID

get the unit id of this drive (0 or 1)

init

used after creating the nub.

MyATACallback

to be deprecated.

processCallback

to be deprecated.

publishBusProperties

puts info about this device's bus capability in the device tree.

publishProperties

publish the nub's properties in the device tree.

publishVendorProperties

will be deprecated.

swapBytes16

to be deprecated.

### DataTypes

ExpansionData

### Instance Variables

reserved

### Instance Methods

- allocCommand

- attach

- executeCommand

- freeCommand

- getDeviceID

- getMetaClass

- init

- processCallback

- publishBusProperties

- publishProperties

- publishVendorProperties

- swapBytes16

### Type Methods

+ MyATACallback

+ ataDeviceNub

## Relationships

### Inherits From

- IOATADevice

## See Also

### Devices

IOATADevice

This object implements a relay to an ATA Bus where a drive is attached.

