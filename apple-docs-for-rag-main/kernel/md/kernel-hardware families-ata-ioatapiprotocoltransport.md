

- Kernel
- Hardware Families
- ATA
-  IOATAPIProtocolTransport 

Class

# IOATAPIProtocolTransport

SCSI Protocol Driver Family for ATAPI Devices.

macOS 11.0+

``` source
class IOATAPIProtocolTransport : IOSCSIProtocolServices
```

## Overview

IOATAPIProtocolTransport contains all the bus specific support for ATAPI compliant devices. To add vendor specific features or workarounds you will sub-class the appropriate methods of this family.

## Topics

### Instance Methods

- AbortSCSICommand

- AllocateATACommandObjects

- CheckWakeupResetOccurred

- CompleteSCSITask

- ConfigureATAPIDevice

- DeallocateATACommandObjects

- DisablePollingOfStatusRegister

- EnablePollingOfStatusRegister

- GatedWaitForRequest

- GetATACommandObject

- HandlePowerOff

- HandlePowerOn

- HandleProtocolServiceFeature

- IdentifyATAPIDevice

- IdentifyAndConfigureATAPIDevice

- InspectDevice

- IsProtocolServiceSupported

- PollStatusRegister

- PollStatusRegisterCallback

- ReconfigureATAPIDevice

- ReportATAPIDeviceType

- ResetATAPIDevice

- ReturnATACommandObject

- SCSITaskCallbackFunction

- SendATASleepCommand

- SendCommand

- SendSCSICommand

- SetDMATransferMode

- SetPIOTransferMode

- SetWakeupResetOccurred

- TurnDrivePowerOff

- free

- getMetaClass

- init

- message

- start

- stop

### Type Methods

+ sATACallbackSync

+ sATAPIConfigStateMachine

+ sATAPIResetCallback

+ sATAPIVoidCallback

+ sCheckWakeupResetOccurred

+ sConvertHighestBitToNumber

+ sPollStatusRegister

+ sPollStatusRegisterCallback

+ sSCSITaskCallbackProc

+ sSetWakeupResetOccurred

+ sSwapBytes16

## Relationships

### Inherits From

- IOSCSIProtocolServices

## See Also

### ATAPI

ATAPIClientData

ATAPICmdPacket

