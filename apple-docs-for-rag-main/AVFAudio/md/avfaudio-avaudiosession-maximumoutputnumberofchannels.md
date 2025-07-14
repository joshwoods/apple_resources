

- AVFAudio
- AVAudioSession
-  maximumOutputNumberOfChannels 

Instance Property

# maximumOutputNumberOfChannels

The maximum number of output channels available for the current audio route.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var maximumOutputNumberOfChannels: Int { get }
```

## See Also

### Setting the number of output channels

var preferredOutputNumberOfChannels: Int

The preferred number of output channels for the current route.

func setPreferredOutputNumberOfChannels(Int) throws

Sets the preferred number of output channels for the current route.

var outputNumberOfChannels: Int

The number of audio output channels.

