

- AudioDriverKit
- IOUserAudioDevice
-  GetPreferredChannelsForStereo 

Instance Method

# GetPreferredChannelsForStereo

Returns the channel indices for the prefered stereo pair.

DriverKit 21.0+

``` source
void GetPreferredChannelsForStereo(uint32_t * out_left_channel, uint32_t * out_right_channel);
```

## Parameters 

`out_left_channel`  

On return, the channel index for the left channel.

`out_right_channel`  

On return, the channel index for the right channel.

## See Also

### Working with Channel Layouts

SetPreferredChannelsForStereo

Sets the channel indices for the prefered stereo pair.

SetPreferredInputChannelLayout

Sets the input channel layout, using an array of audio channel label values.

SetPreferredOutputChannelLayout

Sets the output channel layout, using an array of audio channel label values.

IOUserAudioChannelLabel

Constants to set the preferred channel layout on an audio device.

