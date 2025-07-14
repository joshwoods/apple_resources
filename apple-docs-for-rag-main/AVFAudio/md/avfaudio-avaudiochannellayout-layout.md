

- AVFAudio
- AVAudioChannelLayout
-  layout 

Instance Property

# layout

The underlying audio channel layout.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var layout: UnsafePointer { get }
```

## See Also

### Related Documentation

init(layout: UnsafePointer&lt;AudioChannelLayout>)

Creates an audio channel layout object from an existing one.

### Getting Audio Channel Layout Properties

typealias AVAudioChannelCount

The number of audio channels.

var channelCount: AVAudioChannelCount

The number of channels of audio data.

var layoutTag: AudioChannelLayoutTag

The audio channel’s underlying layout tag.

func isEqual(Any) -> Bool

Indicates whether another audio channel layout is exactly equal to the current layout.

