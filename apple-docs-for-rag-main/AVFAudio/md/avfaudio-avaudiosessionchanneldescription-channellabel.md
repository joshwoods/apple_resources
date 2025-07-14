

- AVFAudio
- AVAudioSessionChannelDescription
-  channelLabel 

Instance Property

# channelLabel

A description of the physical location of this channel.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var channelLabel: AudioChannelLabel { get }
```

## See Also

### Getting the Channel Information

var channelName: String

The descriptive name for the channel.

var channelNumber: Int

The index of this channel in its owning port’s array of channels.

var owningPortUID: String

The unique identifier (UID) for this channel’s owning port.

