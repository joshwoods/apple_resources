

- AudioDriverKit
- IOUserAudioStereoPanControl
-  GetPanningChannels 

Instance Method

# GetPanningChannels

Gets the current stereo panning channels.

DriverKit 21.0+

``` source
void GetPanningChannels(IOUserAudioObjectPropertyElement * out_left_channel, IOUserAudioObjectPropertyElement * out_right_channel);
```

## Parameters 

`out_left_channel`  

On return, the IOUserAudioObjectPropertyElement for the left channel.

`out_right_channel`  

On return, the IOUserAudioObjectPropertyElement for the right channel.

## Discussion

This method synchronizes by using the work queue created by the object.

## See Also

### Accessing the Value

SetControlValue

Sets the stereo pan value of the control.

GetControlValue

Gets the floating-point stereo pan value of the control.

SetPanningChannels

Sets the current stereo panning channels.

