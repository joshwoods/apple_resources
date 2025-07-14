

- AudioDriverKit
-  IOUserAudioLevelControl 

Class

# IOUserAudioLevelControl

A control object that supports setting an audio level, with either scalar or decibel values.

DriverKit 21.0+

``` source
class IOUserAudioLevelControl;
```

## Topics

### Creating a Level Control

Create

Allocates and initializes an instance of the level control class.

init

Initializes an instance of a level control.

IOUserAudioDriver

A DriverKit provider object that manages communications with an audio device.

IOUserAudioLevelControlRange

A type that indicates minimum and maximum values for level controls.

IOUserAudioObjectPropertyElement

A four character code which, along with the selector and scope, identify a specific piece of information about an audio object.

IOUserAudioObjectPropertyScope

A four character code which, along with the selector and element, identify a specific piece of information about an audio object.

### Freeing a Level Control

free

Frees the level control.

### Getting Information About the Class

GetClassID

Gets the audio class identifier of the object.

GetBaseClassID

Gets the audio class identifier of the base class object.

IOUserAudioClassID

An identifier for the type of audio object.

### Supporting Value Changes

HandleChangeScalarValue

Tells the slider control the scalar value is changing.

HandleChangeDecibelValue

Tells the slider control the decibel value is changing.

### Accessing the Value

SetScalarValue

Sets the scalar value of the level control.

GetScalarValue

Gets the scalar value of the level control.

SetDecibelValue

Sets the decibel value of the level control.

GetDecibelValue

Gets the decibel value of the level control.

## Relationships

### Inherits From

- IOUserAudioControl

## See Also

### Using Audio Controls

IOUserAudioControl

The base class for audio control objects.

IOUserAudioBooleanControl

A control object that supports setting a Boolean value.

IOUserAudioStereoPanControl

A control object that supports panning between stereo channels.

IOUserAudioSliderControl

A control object that supports setting a 32-bit integer value.

IOUserAudioSelectorControl

A control object that supports selecting from a set of values.

