

- AVFAudio
- AVAudioSession
-  maximumInputNumberOfChannels 

Instance Property

# maximumInputNumberOfChannels

The maximum number of input channels available for the current audio route.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var maximumInputNumberOfChannels: Int { get }
```

## See Also

### Setting the number of input channels

var preferredInputNumberOfChannels: Int

The preferred number of input channels for the current route.

func setPreferredInputNumberOfChannels(Int) throws

Sets the preferred number of input channels for the current route.

var inputNumberOfChannels: Int

The number of audio input channels for the current route.

