

- AudioDriverKit
- IOUserAudioStereoPanControl
-  SetPanningChannels 

Instance Method

# SetPanningChannels

Sets the current stereo panning channels.

DriverKit 21.0+

``` source
kern_return_t SetPanningChannels(IOUserAudioObjectPropertyElement in_left_channel, IOUserAudioObjectPropertyElement in_right_channel);
```

## Parameters 

`in_left_channel`  

The IOUserAudioObjectPropertyElement for the left channel.

`in_right_channel`  

The IOUserAudioObjectPropertyElement for the right channel.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

If successful, changing the panning channels sends a notification to the host to update the object state.

This method synchronizes by using the work queue created by the object.

## See Also

### Accessing the Value

SetControlValue

Sets the stereo pan value of the control.

GetControlValue

Gets the floating-point stereo pan value of the control.

GetPanningChannels

Gets the current stereo panning channels.

