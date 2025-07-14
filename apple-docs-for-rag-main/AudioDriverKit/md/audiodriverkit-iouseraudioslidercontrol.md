

- AudioDriverKit
-  IOUserAudioSliderControl 

Class

# IOUserAudioSliderControl

A control object that supports setting a 32-bit integer value.

DriverKit 21.0+

``` source
class IOUserAudioSliderControl;
```

## Topics

### Creating a Slider Control

Create

Allocates and initializes an instance of the slider control class.

init

Initializes an instance of a slider control.

IOUserAudioObjectPropertyElement

A four character code which, along with the selector and scope, identify a specific piece of information about an audio object.

IOUserAudioObjectPropertyScope

A four character code which, along with the selector and element, identify a specific piece of information about an audio object.

IOUserAudioDriver

A DriverKit provider object that manages communications with an audio device.

### Freeing a Slider Control

free

Frees the slider control.

### Getting Information About the Class

GetClassID

Gets the audio class identifier of the object.

GetBaseClassID

Gets the audio class identifier of the base class object.

IOUserAudioClassID

An identifier for the type of audio object.

### Supporting Value Changes

HandleChangeControlValue

Tells the slider control the value is changing.

### Accessing the Value

SetControlValue

Sets the value of the slider control.

GetControlValue

Gets the value of the slider control.

SetRange

Sets the range of possible values for the slider.

GetRange

Gets the range of possible values for the slider.

IOUserAudioSliderRange

A type that indicates minimum and maximum values for slider controls.

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

IOUserAudioSelectorControl

A control object that supports selecting from a set of values.

IOUserAudioLevelControl

A control object that supports setting an audio level, with either scalar or decibel values.

