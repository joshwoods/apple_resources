

- AVFAudio
- AVSpeechSynthesisMarker
-  AVSpeechSynthesisMarker.Mark 

Enumeration

# AVSpeechSynthesisMarker.Mark

Constants that describe the type of text.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum Mark
```

## Topics

### Marks

case word

A type of text that represents a word.

case sentence

A type of text that represents a sentence.

case paragraph

A type of text that represents a paragraph.

case phoneme

A type of text that represents a phoneme.

case bookmark

A Speech Synthesis Markup Language (SSML) mark tag.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting a marker

var mark: AVSpeechSynthesisMarker.Mark

The type that describes the text.

var bookmarkName: String

A string that represents the name of a bookmark.

var phoneme: String

A string that represents a distinct sound.

var textRange: NSRange

The location and length of the request’s text.

var byteSampleOffset: Int

The byte offset into the audio buffer.

