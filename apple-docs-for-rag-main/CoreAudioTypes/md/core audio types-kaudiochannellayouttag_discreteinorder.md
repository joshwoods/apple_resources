

- Core Audio Types
-  kAudioChannelLayoutTag_DiscreteInOrder 

Global Variable

# kAudioChannelLayoutTag_DiscreteInOrder

A tag used to map input channels to output channels without changing the channel order.

iOS 2.0+iPadOS 2.0+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var kAudioChannelLayoutTag_DiscreteInOrder: AudioChannelLayoutTag { get }
```

## Discussion

This tag needs to be `OR`ed with the actual number of channels.

## See Also

### General Information Tags

var kAudioChannelLayoutTag_Unknown: AudioChannelLayoutTag

The channel layout is unknown.

