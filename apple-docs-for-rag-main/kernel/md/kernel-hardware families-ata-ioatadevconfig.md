

- Kernel
- Hardware Families
- ATA
-  IOATADevConfig 

Class

# IOATADevConfig

used for configuring and communicating the desired transfer modes of a device. A disk driver would typically use this object in conjunction with the 512-bytes of identification data from the drive and the IOATABusInfo object for the bus it is connected to. This object will determine the best matching transfer speeds available. the device driver will then send a series of Set Features commands to configure the drive and this object to the bus through the IOATADevice nub in order to configure the optimum transfer mode. The driver for the disk drive may choose to populate this object with whatever transfer mode desired, in the event that a different mode is required.

macOS 11.0+

``` source
class IOATADevConfig : OSObject
```

## Overview

usually use the initWithBestSelection to make a best mode match. The Mode accessors use bit significance to indicate a selected mode or supported modes(s) ie, 00000001b indicates Mode-0, 00000010b indicates mode 1, etc. Selected mode is indicated by a single set bit. No bit set indicates no mode in that class is selected. ie, a bus will support multiple possible modes, but will only have one mode selected at that time.

## Topics

### Miscellaneous

atadevconfig

static creator function.

bitSigToNumeric

converts a bit-significant field to a numerical value. Note that a bit field of 0x00 has no defined result.

getDMACycleTime

getDMAMode

getPacketConfig

getPIOCycleTime

getPIOMode

getUltraMode

initWithBestSelection

Handy initializer: pass the 512-byte result of the Identify Device or Identify Packet Device in endian-order for your platform (byte-swapped on PPC) and the IOATABusInfo object for the bus. The object will initialize all fields and select the best transfer modes that match on bus and device. If the return value was 0 (success or noErr), then a matching mode is supported. Examine the PIO and UDMA/DMA fields and to generate the apropriate SET FEATURES parameters for your drive and send this initialised object to the IOATAController when requesting a speed configuration. failure means no supported transfer modes matched between bus and device info.

setDMACycleTime

setDMAMode

setPacketConfig

For ATAPI devices, if the device asserts interrupt after the Packet Command when it is ready to accept the packet, set this value to true (mostly older devices). If the device accepts the packet only by asserting DRQ bit in status, then set this value false. Tells the bus controller whether to wait for packet acceptance or set pending interrupt.

setPIOCycleTime

setPIOMode

setUltraMode

### DataTypes

ExpansionData

### Instance Variables

reserved

### Instance Methods

- assignFromData

- bitSigToNumeric

- getDMACycleTime

- getDMAMode

- getMetaClass

- getPIOCycleTime

- getPIOMode

- getPacketConfig

- getUltraMode

- init

- initWithBestSelection

- setDMACycleTime

- setDMAMode

- setPIOCycleTime

- setPIOMode

- setPacketConfig

- setUltraMode

### Type Methods

+ atadevconfig

+ sDriveExtendedLBASize

+ sDriveSupports48BitLBA

## Relationships

### Inherits From

- OSObject

## See Also

### Base Types

ATAOperationType

ATARequestIdentifier

IOExtendedLBA

If 48-bit LBAs are supported, IOExtendedLBA is used to represent a 48-bit LBA. The driver examines the ATA identify data to determine if 48-bit addressing is supported.

IOATABusInfo

used to indicate the capabilities of the bus the device is connected to, PIO and DMA modes supported, etc.

IOATACompletionFunction

