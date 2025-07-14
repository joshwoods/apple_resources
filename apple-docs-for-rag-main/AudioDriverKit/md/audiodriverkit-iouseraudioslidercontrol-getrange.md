

- AudioDriverKit
- IOUserAudioSliderControl
-  GetRange 

Instance Method

# GetRange

Gets the range of possible values for the slider.

DriverKit 21.0+

``` source
IOUserAudioSliderRange GetRange();
```

## Return Value

The range of possible values for the slider.

## Discussion

This method synchronizes by using the work queue created by the object.

## See Also

### Accessing the Value

SetControlValue

Sets the value of the slider control.

GetControlValue

Gets the value of the slider control.

SetRange

Sets the range of possible values for the slider.

IOUserAudioSliderRange

A type that indicates minimum and maximum values for slider controls.

