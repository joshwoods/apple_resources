

- Kernel
- Hardware Families
- SCSI
-  IOSCSIPeripheralDeviceNub 

Class

# IOSCSIPeripheralDeviceNub

macOS 10.6+

``` source
class IOSCSIPeripheralDeviceNub : IOSCSIProtocolServices
```

## Topics

### Instance Methods

- AbortCommand

- AbortSCSICommand

- AbortTask

- AbortTaskSet

- ClearACA

- ClearTaskSet

- ExecuteCommand

- GatedWaitForTask

- HandleProtocolServiceFeature

- InterrogateDevice

- IsProtocolServiceSupported

- LogicalUnitReset

- SendSCSICommand

- SendTask

- TargetReset

- TaskCompletion

- free

- getMetaClass

- init

- matchPropertyTable

- message

- setProperties

- start

### Type Methods

+ TaskCallback

+ sCompareIOProperty

+ sWaitForTask

## Relationships

### Inherits From

- IOSCSIProtocolServices

## See Also

### Base Types

IOReducedBlockServices

IOSCSIPrimaryCommandsDevice

IOSCSIProtocolServices

This class defines the public SCSI Protocol Services Layer API for any class that implements SCSI protocol services. A protocol services layer driver is responsible for taking incoming SCSITaskIdentifier objects and translating them to the native command type for the native protocol interface (e.g. SBP-2 ORB on FireWire).

IOSCSIProtocolInterface

This class defines the public SCSI Protocol Layer API for any class that provides Protocol services or needs to provide the Protocol Service API for passing service requests to a Protocol Service driver.

