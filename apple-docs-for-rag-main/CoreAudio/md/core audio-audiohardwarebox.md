

- Core Audio
-  AudioHardwareBox 

Class

# AudioHardwareBox

macOS 15.0+

``` source
class AudioHardwareBox
```

## Topics

### Initializers

init(id: AudioObjectID)

### Instance Properties

var clocks: [AudioHardwareClock]

var devices: [AudioHardwareDevice]

var enabled: Bool

var hasAudio: Bool

var hasMIDI: Bool

var hasVideo: Bool

var isProtected: Bool

var transportType: UInt32

var uid: String

### Instance Methods

func disable() throws

func enable() throws

## Relationships

### Inherits From

- AudioHardwareObject

