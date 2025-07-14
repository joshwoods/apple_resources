

- AudioDriverKit
-  IOUserAudioControl 

Class

# IOUserAudioControl

The base class for audio control objects.

DriverKit 21.0+

``` source
class IOUserAudioControl;
```

## Overview

Don’t subclass or allocate this class directly.

## Topics

### Creating a Control

init

Initializes an instance of an audio control.

IOUserAudioDriver

A DriverKit provider object that manages communications with an audio device.

IOUserAudioObjectPropertyElement

A four character code which, along with the selector and scope, identify a specific piece of information about an audio object.

IOUserAudioObjectPropertyScope

A four character code which, along with the selector and element, identify a specific piece of information about an audio object.

### Freeing a Control

free

Frees the audio control.

### Getting Information About the Class

GetClassID

Gets the audio class identifier of the object.

GetBaseClassID

Gets the audio class identifier of the base class object.

IOUserAudioClassID

An identifier for the type of audio object.

### Working with Control Properties

GetControlScope

Returns the control’s scope: input, output, global, or play-through.

IOUserAudioObjectPropertyScope

A four character code which, along with the selector and element, identify a specific piece of information about an audio object.

GetControlElement

Returns the control’s identifying element.

IOUserAudioObjectPropertyElement

A four character code which, along with the selector and scope, identify a specific piece of information about an audio object.

IOUserAudioObjectPropertyElementMain

The identifier for an audio object’s main element.

GetIsSettable

Returns a Boolean value that idicates if the control can be set.

## Relationships

### Inherits From

- IOUserAudioObject

### Inherited By

- IOUserAudioBooleanControl
- IOUserAudioLevelControl
- IOUserAudioSelectorControl
- IOUserAudioSliderControl
- IOUserAudioStereoPanControl

## See Also

### Using Audio Controls

IOUserAudioBooleanControl

A control object that supports setting a Boolean value.

IOUserAudioStereoPanControl

A control object that supports panning between stereo channels.

IOUserAudioSliderControl

A control object that supports setting a 32-bit integer value.

IOUserAudioSelectorControl

A control object that supports selecting from a set of values.

IOUserAudioLevelControl

A control object that supports setting an audio level, with either scalar or decibel values.

