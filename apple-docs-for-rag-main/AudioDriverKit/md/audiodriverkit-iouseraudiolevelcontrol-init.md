

- AudioDriverKit
- IOUserAudioLevelControl
-  init 

Instance Method

# init

Initializes an instance of a level control.

DriverKit 21.0+

``` source
bool init(IOUserAudioDriver * in_driver, bool in_is_settable, float in_decibel_value, IOUserAudioLevelControlRange in_decibel_range, IOUserAudioObjectPropertyElement in_control_element, IOUserAudioObjectPropertyScope in_control_scope, IOUserAudioClassID in_control_class_id);
```

## Parameters 

`in_driver`  

The IOUserAudioDriver that owns this object.

`in_is_settable`  

A Boolean value that indicates if the control can be set.

`in_decibel_value`  

A floating-point value that represents the level control’s current value in decibels.

`in_decibel_range`  

A IOUserAudioLevelControlRange that describes the minimum and maximum values of the level control.

`in_control_element`  

An IOUserAudioObjectPropertyElement to identify the control.

`in_control_scope`  

A IOUserAudioObjectPropertyScope indicating the control’s scope: input, output, global, or play-through.

`in_control_class_id`  

The IOUserAudioClassID of the control.

## Return Value

`true` if initialization succeeded; `false` otherwise.

## See Also

### Creating a Level Control

Create

Allocates and initializes an instance of the level control class.

IOUserAudioDriver

A DriverKit provider object that manages communications with an audio device.

IOUserAudioLevelControlRange

A type that indicates minimum and maximum values for level controls.

IOUserAudioObjectPropertyElement

A four character code which, along with the selector and scope, identify a specific piece of information about an audio object.

IOUserAudioObjectPropertyScope

A four character code which, along with the selector and element, identify a specific piece of information about an audio object.

