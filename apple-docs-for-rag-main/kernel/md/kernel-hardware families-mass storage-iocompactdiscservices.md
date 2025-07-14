

- Kernel
- Hardware Families
- Mass Storage
-  IOCompactDiscServices 

Class

# IOCompactDiscServices

macOS 10.6+

``` source
class IOCompactDiscServices : IOCDBlockStorageDevice
```

## Topics

### Instance Methods

- audioPause

- audioPlay

- audioScan

- audioStop

- doAsyncReadCD

- doAsyncReadWrite

- doAsyncReadWrite

- doAsyncReadWrite

- doEjectMedia

- doFormatMedia

- doGetFormatCapacities

- doSynchronizeCache

- free

- getAdditionalDeviceInfoString

- getAudioStatus

- getAudioVolume

- getMediaType

- getMetaClass

- getProductString

- getRevisionString

- getSpeed

- getVendorString

- getWriteCacheState

- handleClose

- handleIsOpen

- handleOpen

- message

- open

- readDiscInfo

- readISRC

- readMCN

- readTOC

- readTOC

- readTrackInfo

- reportBlockSize

- reportEjectability

- reportMaxValidBlock

- reportMediaState

- reportRemovability

- reportWriteProtection

- setAudioVolume

- setProperties

- setSpeed

- setWriteCacheState

- start

### Type Methods

+ AsyncReadWriteComplete

## Relationships

### Inherits From

- IOCDBlockStorageDevice

## See Also

### Interfaces

IODVDServices

IOBDBlockStorageDevice

The IOBDBlockStorageDevice class is a generic BD block storage device abstraction.

IODVDBlockStorageDevice

The IODVDBlockStorageDevice class is a generic DVD block storage device abstraction.

IOBDMediaBSDClient

IOMediaBSDClient

