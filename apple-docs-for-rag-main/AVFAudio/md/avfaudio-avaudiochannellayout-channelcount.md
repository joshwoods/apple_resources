

- AVFAudio
- AVAudioChannelLayout
-  channelCount 

Instance Property

# channelCount

The number of channels of audio data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var channelCount: AVAudioChannelCount { get }
```

## See Also

### Getting Audio Channel Layout Properties

typealias AVAudioChannelCount

The number of audio channels.

var layout: UnsafePointer&lt;AudioChannelLayout>

The underlying audio channel layout.

var layoutTag: AudioChannelLayoutTag

The audio channel’s underlying layout tag.

func isEqual(Any) -> Bool

Indicates whether another audio channel layout is exactly equal to the current layout.

