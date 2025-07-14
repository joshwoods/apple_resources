

- AudioDriverKit
-  IOUserAudioBooleanControl 

Class

# IOUserAudioBooleanControl

A control object that supports setting a Boolean value.

DriverKit 21.0+

``` source
class IOUserAudioBooleanControl;
```

## Topics

### Creating a Boolean Control

Create

Allocates and initializes an instance of the Boolean control class.

init

Initializes an instance of a Boolean control.

IOUserAudioObjectPropertyElement

A four character code which, along with the selector and scope, identify a specific piece of information about an audio object.

IOUserAudioObjectPropertyScope

A four character code which, along with the selector and element, identify a specific piece of information about an audio object.

### Freeing a Boolean Control

free

Frees the audio Boolean control.

### Getting Information About the Class

GetClassID

Gets the audio class identifier of the object.

GetBaseClassID

Gets the audio class identifier of the base class object.

IOUserAudioClassID

An identifier for the type of audio object.

### Supporting Value Changes

HandleChangeControlValue

Tells the Boolean control the value is changing.

### Accessing the Value

SetControlValue

Sets the Boolean value of the control.

GetControlValue

Gets the Boolean value of the control.

## Relationships

### Inherits From

- IOUserAudioControl

## See Also

### Using Audio Controls

IOUserAudioControl

The base class for audio control objects.

IOUserAudioStereoPanControl

A control object that supports panning between stereo channels.

IOUserAudioSliderControl

A control object that supports setting a 32-bit integer value.

IOUserAudioSelectorControl

A control object that supports selecting from a set of values.

IOUserAudioLevelControl

A control object that supports setting an audio level, with either scalar or decibel values.

