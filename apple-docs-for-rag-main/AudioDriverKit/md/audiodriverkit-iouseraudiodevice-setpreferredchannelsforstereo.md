

- AudioDriverKit
- IOUserAudioDevice
-  SetPreferredChannelsForStereo 

Instance Method

# SetPreferredChannelsForStereo

Sets the channel indices for the prefered stereo pair.

DriverKit 21.0+

``` source
kern_return_t SetPreferredChannelsForStereo(uint32_t in_left_channel, uint32_t in_right_channel);
```

## Parameters 

`in_left_channel`  

The channel index for the left channel.

`in_right_channel`  

The channel index for the right channel.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## See Also

### Working with Channel Layouts

GetPreferredChannelsForStereo

Returns the channel indices for the prefered stereo pair.

SetPreferredInputChannelLayout

Sets the input channel layout, using an array of audio channel label values.

SetPreferredOutputChannelLayout

Sets the output channel layout, using an array of audio channel label values.

IOUserAudioChannelLabel

Constants to set the preferred channel layout on an audio device.

