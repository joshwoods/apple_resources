

- Core Audio
-  AudioHardwareAggregateDevice 

Class

# AudioHardwareAggregateDevice

macOS 15.0+

``` source
class AudioHardwareAggregateDevice
```

## Topics

### Initializers

init(id: AudioObjectID)

### Instance Properties

var activeSubdevices: [AudioHardwareClock]

var activeSubtaps: [AudioHardwareTap]

var clockSource: AudioHardwareObject?

var composition: [String : Any]

var subdevices: [AudioHardwareClock]

var subtaps: [AudioHardwareTap]

### Instance Methods

func setClockSource(AudioHardwareObject) throws

func setComposition([String : Any]) throws

func setSubdevices([AudioHardwareClock]) throws

func setSubtaps([AudioHardwareTap]) throws

## Relationships

### Inherits From

- AudioHardwareDevice

