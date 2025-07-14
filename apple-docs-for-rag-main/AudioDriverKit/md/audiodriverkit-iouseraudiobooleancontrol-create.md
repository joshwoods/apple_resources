

- AudioDriverKit
- IOUserAudioBooleanControl
-  Create 

Static Method

# Create

Allocates and initializes an instance of the Boolean control class.

DriverKit 21.0+

``` source
static OSSharedPtr Create(IOUserAudioDriver * in_driver, bool in_is_settable, bool in_control_value, IOUserAudioObjectPropertyElement in_control_element, IOUserAudioObjectPropertyScope in_control_scope, IOUserAudioClassID in_control_class_id);
```

## Parameters 

`in_driver`  

The IOUserAudioDriver that owns this object.

`in_is_settable`  

A Boolean value that indicates if the control can be set.

`in_control_value`  

A Boolean value that represents the control’s current value.

`in_control_element`  

An IOUserAudioObjectPropertyElement to identify the control.

`in_control_scope`  

A IOUserAudioObjectPropertyScope indicating the control’s scope: input, output, global, or play-through.

`in_control_class_id`  

The IOUserAudioClassID of the control.

## Return Value

A poiner to an IOUserAudioBooleanControl, if allocation and initialization succeeded.

## Discussion

If you subclass IOUserAudioBooleanControl to override this class’ behavior, don’t use Create to allocate and initialize the custom subclass.

## See Also

### Creating a Boolean Control

init

Initializes an instance of a Boolean control.

IOUserAudioObjectPropertyElement

A four character code which, along with the selector and scope, identify a specific piece of information about an audio object.

IOUserAudioObjectPropertyScope

A four character code which, along with the selector and element, identify a specific piece of information about an audio object.

