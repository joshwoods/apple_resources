

- Kernel
- Hardware Families
-  ATA 

API Collection

# ATA

Implement a driver that supports Advanced Technology Attachment (ATA) devices.

## Topics

### Devices

ATADeviceNub

ATADeviceNub is a concrete implementation of IOATADevice.

IOATADevice

This object implements a relay to an ATA Bus where a drive is attached.

### Controller

IOATAController

The base class for ata controller family. Provides the interface common to all ata bus controllers.

### Registers

IOATAReg32

IOATAReg16

IOATAReg8

IOATAIOReg32

IOATAIOReg16

IOATAIOReg8

IOATARegPtr32

IOATARegPtr16

IOATARegPtr8

### Commands

IOATABusCommand64

IOATABusCommand

IOATACommand

### Event Source

ATATimerEventSource

Extend the timer event source to allow checking for timer expiration from behind the workloop.

### ATAPI

IOATAPIProtocolTransport

SCSI Protocol Driver Family for ATAPI Devices.

ATAPIClientData

ATAPICmdPacket

### Base Types

ATAOperationType

ATARequestIdentifier

IOExtendedLBA

If 48-bit LBAs are supported, IOExtendedLBA is used to represent a 48-bit LBA. The driver examines the ATA identify data to determine if 48-bit addressing is supported.

IOATABusInfo

used to indicate the capabilities of the bus the device is connected to, PIO and DMA modes supported, etc.

IOATADevConfig

used for configuring and communicating the desired transfer modes of a device. A disk driver would typically use this object in conjunction with the 512-bytes of identification data from the drive and the IOATABusInfo object for the bus it is connected to. This object will determine the best matching transfer speeds available. the device driver will then send a series of Set Features commands to configure the drive and this object to the bus through the IOATADevice nub in order to configure the optimum transfer mode. The driver for the disk drive may choose to populate this object with whatever transfer mode desired, in the event that a different mode is required.

IOATACompletionFunction

### Additional Types

ataDeviceType

ataEventCode

ataFlags

ataOpcode

ataRegMask

ataSocketType

ataUnitID

atapiConfig

## See Also

### Hardware Interconnects

Bluetooth

Implement a driver that supports Bluetooth devices.

FireWire

Implement a driver that supports FireWire devices.

PCI

Implement a driver that supports Thunderbolt devices or PCI cards.

USB

Implement a driver that supports Universal Serial Bus (USB) devices.

