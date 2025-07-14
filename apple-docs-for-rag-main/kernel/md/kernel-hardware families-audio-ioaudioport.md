

- Kernel
- Hardware Families
- Audio
-  IOAudioPort 

Class

# IOAudioPort

Represents a logical or physical port or functional unit in an audio device.

macOS 10.1+

``` source
class IOAudioPort : IOService
```

## Overview

An IOAudioPort represents an element in the signal chain in the audio device. It may contain one or more controls (represented by IOAudioControl) by which different attributes of the port may be represented and adjusted.

IOAudioPort objects are connected up in the IORegistry in the IOAudioPlane to represent the signal chain of the device. They may be connected to other IOAudioPorts as well as IOAudioEngines to indicate they either feed into or are fed by one of the audio engines (i.e. they provide input to or take output from the computer).

## Topics

### Miscellaneous

addAudioControl

Adds a newly created IOAudioControl instance to the port.

deactivateAudioControls

Called to shut down all of the audio controls for this port.

free

Frees all of the resources allocated by the IOAudioPort.

initWithAttributes

Initializes a newly allocated IOAudioPort instance with the given attributes

start

Called to start a newly created IOAudioPort.

stop

Called when the IOAudioDevice is stopping when it is no longer available.

withAttributes

Allocates a new IOAudioPort instance with the given attributes

### Instance Methods

- addAudioControlDeprecated

- deactivateAudioControlsDeprecated

- freeDeprecated

- getAudioDeviceDeprecated

- getMetaClass

- initWithAttributesDeprecated

- registerServiceDeprecated

- setNameDeprecated

- setSubTypeDeprecated

- setTypeDeprecated

- startDeprecated

- stopDeprecated

### Type Methods

+ withAttributesDeprecated

## Relationships

### Inherits From

- IOService

## See Also

### Interfaces

IOAudioLevelControl

IOAudioSelectorControl

IOAudioToggleControl

IOAudioControl

Represents any controllable attribute of an IOAudioDevice.

IOAudioEngine

Abstract base class for a single audio audio / I/O engine.

IOAudioStream

This class wraps a single sample buffer in an audio driver.

