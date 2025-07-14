

- AudioDriverKit
- IOUserAudioSliderControl
-  SetControlValue 

Instance Method

# SetControlValue

Sets the value of the slider control.

DriverKit 21.0+

``` source
kern_return_t SetControlValue(uint32_t in_control_value);
```

## Parameters 

`in_control_value`  

The slider value to set.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

If successful, changing the control value sends a notification to the host to update the object state.

This method synchronizes by using the work queue created by the object.

## See Also

### Accessing the Value

GetControlValue

Gets the value of the slider control.

SetRange

Sets the range of possible values for the slider.

GetRange

Gets the range of possible values for the slider.

IOUserAudioSliderRange

A type that indicates minimum and maximum values for slider controls.

