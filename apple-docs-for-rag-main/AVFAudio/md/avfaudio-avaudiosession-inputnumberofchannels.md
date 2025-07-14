

- AVFAudio
- AVAudioSession
-  inputNumberOfChannels 

Instance Property

# inputNumberOfChannels

The number of audio input channels for the current route.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var inputNumberOfChannels: Int { get }
```

## Discussion

You can observe changes to the value of this property by using key-value observing. For more information, see Using Key-Value Observing in Swift.

## See Also

### Setting the number of input channels

var preferredInputNumberOfChannels: Int

The preferred number of input channels for the current route.

func setPreferredInputNumberOfChannels(Int) throws

Sets the preferred number of input channels for the current route.

var maximumInputNumberOfChannels: Int

The maximum number of input channels available for the current audio route.

