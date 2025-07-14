

- Kernel
- Hardware Families
- SCSI
-  IOReducedBlockServices 

Class

# IOReducedBlockServices

macOS 10.6+

``` source
class IOReducedBlockServices : IOBlockStorageDevice
```

## Topics

### Instance Methods

- attach

- detach

- doAsyncReadWrite

- doAsyncReadWrite

- doAsyncReadWrite

- doEjectMedia

- doFormatMedia

- doGetFormatCapacities

- doSynchronizeCache

- free

- getAdditionalDeviceInfoString

- getMetaClass

- getProductString

- getRevisionString

- getVendorString

- getWriteCacheState

- message

- reportBlockSize

- reportEjectability

- reportMaxValidBlock

- reportMediaState

- reportRemovability

- reportWriteProtection

- setWriteCacheState

### Type Methods

+ AsyncReadWriteComplete

## Relationships

### Inherits From

- IOBlockStorageDevice

## See Also

### Base Types

IOSCSIPeripheralDeviceNub

IOSCSIPrimaryCommandsDevice

IOSCSIProtocolServices

This class defines the public SCSI Protocol Services Layer API for any class that implements SCSI protocol services. A protocol services layer driver is responsible for taking incoming SCSITaskIdentifier objects and translating them to the native command type for the native protocol interface (e.g. SBP-2 ORB on FireWire).

IOSCSIProtocolInterface

This class defines the public SCSI Protocol Layer API for any class that provides Protocol services or needs to provide the Protocol Service API for passing service requests to a Protocol Service driver.

