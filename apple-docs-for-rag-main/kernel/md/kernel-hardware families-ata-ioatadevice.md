

- Kernel
- Hardware Families
- ATA
-  IOATADevice 

Class

# IOATADevice

This object implements a relay to an ATA Bus where a drive is attached.

macOS 11.0+

``` source
class IOATADevice : IOService
```

## Overview

IOATADevice is the superclass which represents a particular device attached to a particular IOATAController (bus). IOATADevice is the provider for ATA mass-storage device drivers.IOATADevice is the factory for all IOATACommand objects and is responsible for creating and freeing IOATACommands. IOATAControllers will create an instance of IOATADevice for each device physically connected to the ata bus. IOATADevice is virtual and specific subclass should be implemented for particular types of IOATAController. In this manner, controller-specifc IOATACommands may be paired with the proper type of controller.

## Topics

### Miscellaneous

allocCommand

create IOATACommands. Device drivers should allocate command objects only through this method.

executeCommand

Submit IO requests

freeCommand

release a command object that is no longer needed. Do not free an object in use and do not release the object anymore times than you have retained it.

getDeviceType

Find out what kind of device this nub is (ata or atapi)

getUnitID

Determine whether this device is number 0 or 1 (ie, primary/secondary)

matchLocation

matching stuff for IOBSDInit and so on.

matchPropertyTable(OSDictionary *)

matching stuff for IOBSDInit and so on.

matchPropertyTable(OSDictionary *, SInt32 *)

matching stuff for IOBSDInit and so on.

notifyEvent

called by controllers when they need to send a message to client (disk) drivers.

provideBusInfo

Find out the bus capability so the client can choose the features to set and commands to run.

provideConfig

Find out what speed the bus has configured for this unit.

selectConfig

Tell the bus what speed to use for your device.

### DataTypes

ExpansionData

### Instance Variables

reserved

### Instance Methods

- allocCommand

- executeCommand

- freeCommand

- getDeviceType

- getMetaClass

- getUnitID

- matchLocation

- matchPropertyTable

- matchPropertyTable

- notifyEvent

- provideBusInfo

- provideConfig

- selectConfig

## Relationships

### Inherits From

- IOService

## See Also

### Devices

ATADeviceNub

ATADeviceNub is a concrete implementation of IOATADevice.

