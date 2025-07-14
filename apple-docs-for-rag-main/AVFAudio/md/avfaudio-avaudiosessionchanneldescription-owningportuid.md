

- AVFAudio
- AVAudioSessionChannelDescription
-  owningPortUID 

Instance Property

# owningPortUID

The unique identifier (UID) for this channel’s owning port.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var owningPortUID: String { get }
```

## Discussion

You can use the value of this property along with the value of the channelNumber property to communicate with specific hardware channels.

## See Also

### Getting the Channel Information

var channelName: String

The descriptive name for the channel.

var channelNumber: Int

The index of this channel in its owning port’s array of channels.

var channelLabel: AudioChannelLabel

A description of the physical location of this channel.

