

- Kernel
- Hardware Families
- ATA
-  IOExtendedLBA 

Class

# IOExtendedLBA

If 48-bit LBAs are supported, IOExtendedLBA is used to represent a 48-bit LBA. The driver examines the ATA identify data to determine if 48-bit addressing is supported.

macOS 11.0+

``` source
class IOExtendedLBA : OSObject
```

## Topics

### Miscellaneous

getCommand

Taskfile access. Registers are named in accordance with ATA Standards conventions

getDevice

Taskfile access. Registers are named in accordance with ATA Standards conventions

getExtendedLBA

convenience method that gets a 48-bit LBA

getFeatures16

Taskfile access. Registers are named in accordance with ATA Standards conventions

getLBAHigh16

convenience method that gets the high 16 bits of a 48-bit LBA

getLBALow16

convenience method that gets the lower 16 bits of a 48-bit LBA

getLBAMid16

convenience method that gets the middle 16 bits of a 48-bit LBA

getSectorCount16

Taskfile access. Registers are named in accordance with ATA Standards conventions

setCommand

Taskfile access. Registers are named in accordance with ATA Standards conventions

setDevice

Taskfile access. Registers are named in accordance with ATA Standards conventions

setExtendedLBA

convenience method that sets the taskfile registers into a 48-bit LBA address, along with sector count, and unit selected and LBA bit set

setFeatures16

Taskfile access. Registers are named in accordance with ATA Standards conventions

setLBAHigh16

convenience method that sets the high 16 bits of a 48-bit LBA

setLBALow16

convenience method that sets the lower 16 bits of a 48-bit LBA

setLBAMid16

convenience method that sets the middle 16 bits of a 48-bit LBA

setSectorCount16

Taskfile access. Registers are named in accordance with ATA Standards conventions

zeroData

convenience method that zeros out the lba, sector count, features, device, and command member variables

### DataTypes

ExpansionData

### Instance Variables

reserved

### Instance Methods

- getCommand

- getDevice

- getExtendedLBA

- getFeatures16

- getLBAHigh16

- getLBALow16

- getLBAMid16

- getMetaClass

- getSectorCount16

- setCommand

- setDevice

- setExtendedLBA

- setFeatures16

- setLBAHigh16

- setLBALow16

- setLBAMid16

- setSectorCount16

- zeroData

### Type Methods

+ createIOExtendedLBA

## Relationships

### Inherits From

- OSObject

## See Also

### Base Types

ATAOperationType

ATARequestIdentifier

IOATABusInfo

used to indicate the capabilities of the bus the device is connected to, PIO and DMA modes supported, etc.

IOATADevConfig

used for configuring and communicating the desired transfer modes of a device. A disk driver would typically use this object in conjunction with the 512-bytes of identification data from the drive and the IOATABusInfo object for the bus it is connected to. This object will determine the best matching transfer speeds available. the device driver will then send a series of Set Features commands to configure the drive and this object to the bus through the IOATADevice nub in order to configure the optimum transfer mode. The driver for the disk drive may choose to populate this object with whatever transfer mode desired, in the event that a different mode is required.

IOATACompletionFunction

