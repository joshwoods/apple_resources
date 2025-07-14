

- AVFAudio
- AVAudioChannelLayout
-  isEqual(\_:) 

Instance Method

# isEqual(\_:)

Indicates whether another audio channel layout is exactly equal to the current layout.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isEqual(_ object: Any) -> Bool
```

## Parameters 

`object`  

The audio channel layout object to compare.

## Return Value

A value of true indicates whether they are equal; otherwise, false.

## See Also

### Getting Audio Channel Layout Properties

typealias AVAudioChannelCount

The number of audio channels.

var channelCount: AVAudioChannelCount

The number of channels of audio data.

var layout: UnsafePointer&lt;AudioChannelLayout>

The underlying audio channel layout.

var layoutTag: AudioChannelLayoutTag

The audio channel’s underlying layout tag.

