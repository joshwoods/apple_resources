

- AVFAudio
- AVAudioPlayer
-  channelAssignments 

Instance Property

# channelAssignments

An array of channel descriptions for the audio player.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var channelAssignments: [AVAudioSessionChannelDescription]? { get set }
```

## Discussion

The default value for this property is `nil`. When the value is non-`nil`, this array must have the same number of channels the numberOfChannels property returns. You can use this property to assign output to play to different channels.

## See Also

### Managing audio channels

var numberOfChannels: Int

The number of audio channels in the player’s audio.

