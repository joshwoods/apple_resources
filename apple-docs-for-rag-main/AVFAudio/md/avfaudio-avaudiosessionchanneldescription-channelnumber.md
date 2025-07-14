

- AVFAudio
- AVAudioSessionChannelDescription
-  channelNumber 

Instance Property

# channelNumber

The index of this channel in its owning port’s array of channels.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var channelNumber: Int { get }
```

## Discussion

You can use the value in this property to identify the channel during audio routing. However, the value of this property isn’t guaranteed to persist across route changes.

## See Also

### Getting the Channel Information

var channelName: String

The descriptive name for the channel.

var owningPortUID: String

The unique identifier (UID) for this channel’s owning port.

var channelLabel: AudioChannelLabel

A description of the physical location of this channel.

