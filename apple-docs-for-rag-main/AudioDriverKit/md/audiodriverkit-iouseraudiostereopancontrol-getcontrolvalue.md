

- AudioDriverKit
- IOUserAudioStereoPanControl
-  GetControlValue 

Instance Method

# GetControlValue

Gets the floating-point stereo pan value of the control.

DriverKit 21.0+

``` source
float GetControlValue();
```

## Return Value

The floating-point stereo pan value of the control.

## Discussion

This method synchronizes by using the work queue created by the object.

## See Also

### Accessing the Value

SetControlValue

Sets the stereo pan value of the control.

SetPanningChannels

Sets the current stereo panning channels.

GetPanningChannels

Gets the current stereo panning channels.

