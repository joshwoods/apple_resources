

- AVFAudio
- AVAudioSession
-  preferredOutputNumberOfChannels 

Instance Property

# preferredOutputNumberOfChannels

The preferred number of output channels for the current route.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
var preferredOutputNumberOfChannels: Int { get }
```

## Discussion

The value of this property indicates the preferred number of output channels selected using the setPreferredOutputNumberOfChannels(_:) method.

To determine the actual number of channels, query the outputNumberOfChannels property.

## See Also

### Setting the number of output channels

func setPreferredOutputNumberOfChannels(Int) throws

Sets the preferred number of output channels for the current route.

var outputNumberOfChannels: Int

The number of audio output channels.

var maximumOutputNumberOfChannels: Int

The maximum number of output channels available for the current audio route.

