

- AudioDriverKit
- IOUserAudioDevice
-  SetPreferredOutputChannelLayout 

Instance Method

# SetPreferredOutputChannelLayout

Sets the output channel layout, using an array of audio channel label values.

DriverKit 21.0+

``` source
kern_return_t SetPreferredOutputChannelLayout(IOUserAudioChannelLabel * in_channel_labels, size_t in_num_channels);
```

## Parameters 

`in_channel_labels`  

An array of IOUserAudioChannelLabel values.

`in_num_channels`  

The number of items in the `in_channel_labels` array.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## See Also

### Working with Channel Layouts

SetPreferredChannelsForStereo

Sets the channel indices for the prefered stereo pair.

GetPreferredChannelsForStereo

Returns the channel indices for the prefered stereo pair.

SetPreferredInputChannelLayout

Sets the input channel layout, using an array of audio channel label values.

IOUserAudioChannelLabel

Constants to set the preferred channel layout on an audio device.

