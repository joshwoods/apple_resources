

- AudioDriverKit
-  IOUserAudioLevelControlRange 

Structure

# IOUserAudioLevelControlRange

A type that indicates minimum and maximum values for level controls.

DriverKit 21.0+

``` source
struct IOUserAudioLevelControlRange;
```

## Topics

### Accessing the Minimum and Maximum

m_min

The minimum value of the range.

m_max

The maximum value of the range.

## See Also

### Creating a Level Control

Create

Allocates and initializes an instance of the level control class.

init

Initializes an instance of a level control.

IOUserAudioDriver

A DriverKit provider object that manages communications with an audio device.

IOUserAudioObjectPropertyElement

A four character code which, along with the selector and scope, identify a specific piece of information about an audio object.

IOUserAudioObjectPropertyScope

A four character code which, along with the selector and element, identify a specific piece of information about an audio object.

