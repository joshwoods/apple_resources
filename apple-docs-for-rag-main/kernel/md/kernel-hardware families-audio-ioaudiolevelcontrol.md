

- Kernel
- Hardware Families
- Audio
-  IOAudioLevelControl 

Class

# IOAudioLevelControl

macOS 10.1+

``` source
class IOAudioLevelControl : IOAudioControl
```

## Topics

### Miscellaneous

create

Allocates a new level control with the given attributes

init

Initializes a newly allocated IOAudioLevelControl with the given attributes

setLinearScale

This function tells CoreAudio if it should apply a curve to the scaler representation of the volume.

setMaxDB

Sets the maximum value in db that the control may have

setMaxValue

Sets the maximum value the control may have

setMinDB

Sets the minimum value in db that the control may have

setMinValue

Sets the minimum value the control may have

### Instance Methods

- addNegativeInfinityDeprecated

- addRangeDeprecated

- freeDeprecated

- getMaxDBDeprecated

- getMaxValueDeprecated

- getMetaClass

- getMinDBDeprecated

- getMinValueDeprecated

- initDeprecated

- setLinearScaleDeprecated

- setMaxDBDeprecated

- setMaxValueDeprecated

- setMinDBDeprecated

- setMinValueDeprecated

- validateValueDeprecated

### Type Methods

+ createDeprecated

+ createPassThruVolumeControlDeprecated

+ createVolumeControlDeprecated

## Relationships

### Inherits From

- IOAudioControl

## See Also

### Interfaces

IOAudioSelectorControl

IOAudioToggleControl

IOAudioControl

Represents any controllable attribute of an IOAudioDevice.

IOAudioEngine

Abstract base class for a single audio audio / I/O engine.

IOAudioStream

This class wraps a single sample buffer in an audio driver.

IOAudioPort

Represents a logical or physical port or functional unit in an audio device.

