

- AVFAudio
- AVAudioSession
-  setPreferredOutputNumberOfChannels(\_:) 

Instance Method

# setPreferredOutputNumberOfChannels(\_:)

Sets the preferred number of output channels for the current route.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
func setPreferredOutputNumberOfChannels(_ count: Int) throws
```

## Parameters 

`count`  

The number of output channels you want to use.

## Discussion

This method requests a change to the number of output channels. To determine whether the change has taken effect, use the outputNumberOfChannels property. For details, see Configuring standard audio behaviors. Requesting output channels less than one or greater than that returned by the maximumOutputNumberOfChannels results in an error. Only certain devices and peripherals support this feature.

Set the preferred number of output channels only after setting the audio session’s category and mode, and activating the session.

## See Also

### Setting the number of output channels

var preferredOutputNumberOfChannels: Int

The preferred number of output channels for the current route.

var outputNumberOfChannels: Int

The number of audio output channels.

var maximumOutputNumberOfChannels: Int

The maximum number of output channels available for the current audio route.

