

- Kernel
- Hardware Families
- Mass Storage
-  IODVDServices 

Class

# IODVDServices

macOS 10.6+

``` source
class IODVDServices : IODVDBlockStorageDevice
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

- readDVDStructure

- readDiscInfo

- readISRC

- readMCN

- readTOC

- readTOC

- readTrackInfo

- reportBlockSize

- reportEjectability

- reportKeyDeprecated

- reportKey

- reportMaxValidBlock

- reportMediaState

- reportRemovability

- reportWriteProtection

- requestIdle

- sendKey

- setAudioVolume

- setProperties

- setSpeed

- setWriteCacheState

- start

### Type Methods

+ AsyncReadWriteComplete

## Relationships

### Inherits From

- IODVDBlockStorageDevice

## See Also

### Interfaces

IOBDBlockStorageDevice

The IOBDBlockStorageDevice class is a generic BD block storage device abstraction.

IODVDBlockStorageDevice

The IODVDBlockStorageDevice class is a generic DVD block storage device abstraction.

IOCompactDiscServices

IOBDMediaBSDClient

IOMediaBSDClient

