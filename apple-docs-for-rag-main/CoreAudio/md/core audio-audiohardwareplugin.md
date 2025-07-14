

- Core Audio
-  AudioHardwarePlugin 

Class

# AudioHardwarePlugin

macOS 15.0+

``` source
class AudioHardwarePlugin
```

## Topics

### Initializers

init(id: AudioObjectID)

### Instance Properties

var boxes: [AudioHardwareBox]

var bundleID: String

var clocks: [AudioHardwareClock]

var devices: [AudioHardwareDevice]

### Instance Methods

func box(forUID: String) throws -> AudioHardwareBox?

func clock(forUID: String) throws -> AudioHardwareClock?

func device(forUID: String) throws -> AudioHardwareDevice?

## Relationships

### Inherits From

- AudioHardwareObject

