

- AVFAudio
- AVAudioChannelLayout
-  layoutTag 

Instance Property

# layoutTag

The audio channel’s underlying layout tag.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var layoutTag: AudioChannelLayoutTag { get }
```

## See Also

### Related Documentation

convenience init?(layoutTag: AudioChannelLayoutTag)

Creates an audio channel layout object from a layout tag.

### Getting Audio Channel Layout Properties

typealias AVAudioChannelCount

The number of audio channels.

var channelCount: AVAudioChannelCount

The number of channels of audio data.

var layout: UnsafePointer&lt;AudioChannelLayout>

The underlying audio channel layout.

func isEqual(Any) -> Bool

Indicates whether another audio channel layout is exactly equal to the current layout.

