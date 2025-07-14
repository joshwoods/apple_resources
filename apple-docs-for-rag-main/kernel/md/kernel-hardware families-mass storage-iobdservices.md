

- Kernel
- Hardware Families
- Mass Storage
-  IOBDServices 

Class

# IOBDServices

macOS 10.6+

``` source
class IOBDServices : IOBDBlockStorageDevice
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

- readDiscStructure

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

- splitTrack

- start

### Type Methods

+ AsyncReadWriteComplete

## Relationships

### Inherits From

- IOBDBlockStorageDevice

## See Also

### Devices

IOBlockStorageServices

IOCDBlockStorageDevice

The IOCDBlockStorageDevice class is a generic CD block storage device abstraction.

IOBlockStorageDevice

A generic block storage device abstraction.

