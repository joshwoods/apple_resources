

- Core Audio
-  AudioHardwareStream 

Class

# AudioHardwareStream

macOS 15.0+

``` source
class AudioHardwareStream
```

## Topics

### Initializers

init(id: AudioObjectID)

### Instance Properties

var availablePhysicalFormats: [AudioStreamRangedDescription]

var availableVirtualFormats: [AudioStreamRangedDescription]

var direction: AudioHardwareDirection

var isActive: Bool

var latency: Int

var physicalFormat: AudioStreamBasicDescription

var startingChannel: Int

var terminalType: UInt32

var virtualFormat: AudioStreamBasicDescription

### Instance Methods

func setIsActive(Bool) throws

func setPhysicalFormat(AudioStreamBasicDescription) throws

func setVirtualFormat(AudioStreamBasicDescription) throws

## Relationships

### Inherits From

- AudioHardwareObject

