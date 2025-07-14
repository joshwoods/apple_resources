

- Core Audio
-  AudioHardwareControl 

Class

# AudioHardwareControl

macOS 15.0+

``` source
class AudioHardwareControl
```

## Topics

### Initializers

init(id: AudioObjectID)

### Instance Properties

var availableItems: [UInt32]

var booleanValue: Bool

var selectedItems: [UInt32]

var sliderRange: [UInt32]

var sliderValue: UInt32

var stereoPanChannels: [UInt32]

var stereoPanValue: Float

var volumeDecibelRange: AudioValueRange

var volumeDecibelValue: Float

var volumeScalarValue: Float

### Instance Methods

func convertToDecibels(fromScalar: Float) throws -> Float

func convertToScalar(fromDecibels: Float) throws -> Float

func selectorItemKind(fromID: UInt32) throws -> UInt32

func selectorItemName(fromID: UInt32) throws -> String

func setBooleanValue(Bool) throws

func setSelectedItems([UInt32]) throws

func setSliderValue(UInt32) throws

func setStereoPanValue(Float) throws

func setVolumeDecibelValue(Float) throws

func setVolumeScalarValue(Float) throws

## Relationships

### Inherits From

- AudioHardwareObject

