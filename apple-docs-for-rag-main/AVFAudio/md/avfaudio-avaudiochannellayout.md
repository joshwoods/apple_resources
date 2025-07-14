

- AVFAudio
-  AVAudioChannelLayout 

Class

# AVAudioChannelLayout

An object that describes the roles of a set of audio channels.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVAudioChannelLayout
```

## Overview

The `AVAudioChannelLayout` class is a thin wrapper for Core Audio’s AudioChannelLayout.

## Topics

### Creating an Audio Channel Layout

init(layout: UnsafePointer&lt;AudioChannelLayout>)

Creates an audio channel layout object from an existing one.

convenience init?(layoutTag: AudioChannelLayoutTag)

Creates an audio channel layout object from a layout tag.

### Getting Audio Channel Layout Properties

typealias AVAudioChannelCount

The number of audio channels.

var channelCount: AVAudioChannelCount

The number of channels of audio data.

var layout: UnsafePointer&lt;AudioChannelLayout>

The underlying audio channel layout.

var layoutTag: AudioChannelLayoutTag

The audio channel’s underlying layout tag.

func isEqual(Any) -> Bool

Indicates whether another audio channel layout is exactly equal to the current layout.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Formats

class AVAudioFormat

An object that describes the representation of an audio format.

let AVChannelLayoutKey: String

Linear PCM Format Settings

The audio settings that apply to linear PCM audio formats.

Format Settings

The audio settings that apply to all audio formats that the audio player and recorder classes support.

