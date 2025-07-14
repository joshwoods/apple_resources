

- AVFAudio
- AVAudioSession
-  preferredInputNumberOfChannels 

Instance Property

# preferredInputNumberOfChannels

The preferred number of input channels for the current route.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
var preferredInputNumberOfChannels: Int { get }
```

## Discussion

The value of this property indicates the number of channels selected using the setPreferredInputNumberOfChannels(_:) method.

To determine the actual number of input channels, query the inputNumberOfChannels property.

## See Also

### Setting the number of input channels

func setPreferredInputNumberOfChannels(Int) throws

Sets the preferred number of input channels for the current route.

var inputNumberOfChannels: Int

The number of audio input channels for the current route.

var maximumInputNumberOfChannels: Int

The maximum number of input channels available for the current audio route.

