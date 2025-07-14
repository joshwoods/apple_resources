

- Core Audio
-  AudioHardwareClock 

Class

# AudioHardwareClock

macOS 15.0+

``` source
class AudioHardwareClock
```

## Topics

### Initializers

init(id: AudioObjectID)

### Instance Properties

var availableNominalSampleRates: [AudioValueRange]

var clockDomain: UInt32

var controls: [AudioHardwareControl]

var inputLatency: Int

var isAlive: Bool

var isRunning: Bool

var nominalSampleRate: Double

var outputLatency: Int

var transportType: UInt32

var uid: String

### Instance Methods

func setNominalSampleRate(Double) throws

## Relationships

### Inherits From

- AudioHardwareObject

### Inherited By

- AudioHardwareDevice

