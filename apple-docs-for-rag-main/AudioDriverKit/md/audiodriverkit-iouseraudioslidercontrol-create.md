

- AudioDriverKit
- IOUserAudioSliderControl
-  Create 

Static Method

# Create

Allocates and initializes an instance of the slider control class.

DriverKit 21.0+

``` source
static OSSharedPtr Create(IOUserAudioDriver * in_driver, bool in_is_settable, uint32_t in_control_value, IOUserAudioSliderRange in_range, IOUserAudioObjectPropertyElement in_control_element, IOUserAudioObjectPropertyScope in_control_scope, IOUserAudioClassID in_control_class_id);
```

## Parameters 

`in_driver`  

The IOUserAudioDriver that owns this object.

`in_is_settable`  

A Boolean value that indicates if the control can be set.

`in_control_value`  

A uint32_t value that represents the control’s current value.

`in_range`  

The range that defines minimum and maximum values for the slider.

`in_control_element`  

An IOUserAudioObjectPropertyElement to identify the control.

`in_control_scope`  

A IOUserAudioObjectPropertyScope indicating the control’s scope: input, output, global, or play-through.

`in_control_class_id`  

The IOUserAudioClassID of the control.

## Return Value

A poiner to an IOUserAudioSliderControl, if allocation and initialization succeeded.

## Discussion

If you subclass IOUserAudioSliderControl to override this class’ behavior, don’t use Create to allocate and initialize the custom subclass.

## See Also

### Creating a Slider Control

init

Initializes an instance of a slider control.

IOUserAudioObjectPropertyElement

A four character code which, along with the selector and scope, identify a specific piece of information about an audio object.

IOUserAudioObjectPropertyScope

A four character code which, along with the selector and element, identify a specific piece of information about an audio object.

IOUserAudioDriver

A DriverKit provider object that manages communications with an audio device.

