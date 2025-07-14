

- Kernel
- Hardware Families
- ATA
-  IOATABusInfo 

Class

# IOATABusInfo

used to indicate the capabilities of the bus the device is connected to, PIO and DMA modes supported, etc.

macOS 11.0+

``` source
class IOATABusInfo : OSObject
```

## Topics

### Miscellaneous

atabusinfo

factory method

getDMAModes

bit-significant map of DMA mode(s) supported on the bus. Used by clients of ATAControllers to find out about the bus.

getPIOModes

returns the bit-significant map of PIO mode(s) supported on the bus. Used by clients of ATAControllers to find out about the bus.

getSocketType

returns the socket type, internal fixed, media-bay, PC-Card Used by clients of ATAControllers to find out about the bus

getUltraModes

bit-significant map of Ultra mode(s) supported on the bus. Used by clients of ATAControllers to find out about the bus.

getUnits

How many devices are present on bus. Used by clients of ATAControllers to find out about the bus.

maxBlocksExtended

The maximum number of 512-byte blocks this controller supports in a single Extended LBA transfer. Some controllers may be limited to less than the maximum sector count allowed under extended LBA protocol.

setDMAModes

Bit significant map of supported transfer modes. Set by ATAControllers.

setDMAQueued

Set true if supports DMA Queued Feature. Set by ATAControllers.

setExtendedLBA

Set true for supports 48-bit LBA. Set by ATAControllers.

setMaxBlocksExtended

value set by controllers to indicate the maximum number of blocks allowed in a single transfer of data. Some dma engines may not be capable of supporting the full 16-bit worth of sector count allowed under 48 bit extended LBA. Default is 256 blocks, same as standard ATA.

setOverlapped

Set true for supports overlapped packet feature set. Set by ATAControllers.

setPIOModes

Bit significant map of supported transfer modes. Set by ATAControllers.

setSocketType

internal fixed, media-bay, PC-Card. Set by ATAControllers.

setUltraModes

Bit significant map of supported transfer modes. Set by ATAControllers.

setUnits

set to indicate how many devices are on this bus. Set by ATAControllers.

supportsDMA

True = DMA supported on bus - inferred by looking at the DMA mode bits. Used by clients of ATAControllers to find out about the bus.

supportsDMAQueued

Supports DMA Queued Feature set if true. Used by clients of ATAControllers to find out about the bus.

supportsExtendedLBA

Supports 48-bit LBA if true. Used by clients of ATAControllers to find out about the bus.

supportsOverlapped

Supports overlapped packet feature set if true. Used by clients of ATAControllers to find out about the bus.

zeroData

set this object to a blank state.

### DataTypes

ExpansionData

### Instance Variables

reserved

### Instance Methods

- getDMAModes

- getMetaClass

- getPIOModes

- getSocketType

- getUltraModes

- getUnits

- init

- maxBlocksExtended

- setDMAModes

- setDMAQueued

- setExtendedLBA

- setMaxBlocksExtended

- setOverlapped

- setPIOModes

- setSocketType

- setUltraModes

- setUnits

- supportsDMA

- supportsDMAQueued

- supportsExtendedLBA

- supportsOverlapped

- zeroData

### Type Methods

+ atabusinfo

## Relationships

### Inherits From

- OSObject

## See Also

### Base Types

ATAOperationType

ATARequestIdentifier

IOExtendedLBA

If 48-bit LBAs are supported, IOExtendedLBA is used to represent a 48-bit LBA. The driver examines the ATA identify data to determine if 48-bit addressing is supported.

IOATADevConfig

used for configuring and communicating the desired transfer modes of a device. A disk driver would typically use this object in conjunction with the 512-bytes of identification data from the drive and the IOATABusInfo object for the bus it is connected to. This object will determine the best matching transfer speeds available. the device driver will then send a series of Set Features commands to configure the drive and this object to the bus through the IOATADevice nub in order to configure the optimum transfer mode. The driver for the disk drive may choose to populate this object with whatever transfer mode desired, in the event that a different mode is required.

IOATACompletionFunction

