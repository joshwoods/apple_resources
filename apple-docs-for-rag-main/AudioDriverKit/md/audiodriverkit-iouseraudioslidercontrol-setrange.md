

- AudioDriverKit
- IOUserAudioSliderControl
-  SetRange 

Instance Method

# SetRange

Sets the range of possible values for the slider.

DriverKit 21.0+

``` source
kern_return_t SetRange(IOUserAudioSliderRange in_range);
```

## Parameters 

`in_range`  

The range to set.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

If successful, changing the range sends a notification to the host to update the object state.

This method synchronizes by using the work queue created by the object.

## See Also

### Accessing the Value

SetControlValue

Sets the value of the slider control.

GetControlValue

Gets the value of the slider control.

GetRange

Gets the range of possible values for the slider.

IOUserAudioSliderRange

A type that indicates minimum and maximum values for slider controls.

