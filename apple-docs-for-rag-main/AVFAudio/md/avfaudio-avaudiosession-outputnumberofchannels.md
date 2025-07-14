

- AVFAudio
- AVAudioSession
-  outputNumberOfChannels 

Instance Property

# outputNumberOfChannels

The number of audio output channels.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var outputNumberOfChannels: Int { get }
```

## Discussion

You can observe changes to the value of this property using key-value observice. For more information, see Using Key-Value Observing in Swift.

## See Also

### Setting the number of output channels

var preferredOutputNumberOfChannels: Int

The preferred number of output channels for the current route.

func setPreferredOutputNumberOfChannels(Int) throws

Sets the preferred number of output channels for the current route.

var maximumOutputNumberOfChannels: Int

The maximum number of output channels available for the current audio route.

