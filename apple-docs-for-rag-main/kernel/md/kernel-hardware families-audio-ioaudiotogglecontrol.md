

- Kernel
- Hardware Families
- Audio
-  IOAudioToggleControl 

Class

# IOAudioToggleControl

macOS 10.1+

``` source
class IOAudioToggleControl : IOAudioControl
```

## Topics

### Miscellaneous

create

Allocates a new mute control with the given attributes

createPassThruMuteControl

Allocates a new pass through mute control with the given attributes

init

Initializes a newly allocated IOAudioToggleControl with the given attributes

### Instance Methods

- getMetaClass

- initDeprecated

### Type Methods

+ createDeprecated

+ createMuteControlDeprecated

+ createPassThruMuteControlDeprecated

## Relationships

### Inherits From

- IOAudioControl

## See Also

### Interfaces

IOAudioLevelControl

IOAudioSelectorControl

IOAudioControl

Represents any controllable attribute of an IOAudioDevice.

IOAudioEngine

Abstract base class for a single audio audio / I/O engine.

IOAudioStream

This class wraps a single sample buffer in an audio driver.

IOAudioPort

Represents a logical or physical port or functional unit in an audio device.

