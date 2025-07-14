

- AVFAudio
-  AVSpeechSynthesisMarker 

Class

# AVSpeechSynthesisMarker

An object that contains information about the synthesized audio.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
class AVSpeechSynthesisMarker
```

## Topics

### Creating a marker

init(markerType: AVSpeechSynthesisMarker.Mark, forTextRange: NSRange, atByteSampleOffset: Int)

Creates a marker with a type and location of the request’s text.

init(wordRange: NSRange, atByteSampleOffset: Int)

Creates a word marker with a range of the word and offset into the audio buffer.

init(sentenceRange: NSRange, atByteSampleOffset: Int)

Creates a sentence marker with a range of the sentence and offset into the audio buffer.

init(paragraphRange: NSRange, atByteSampleOffset: Int)

Creates a paragraph marker with a range of the paragraph and offset into the audio buffer.

init(phonemeString: String, atByteSampleOffset: Int)

Creates a phoneme marker with a range of the phoneme and offset into the audio buffer.

init(bookmarkName: String, atByteSampleOffset: Int)

Creates a bookmark marker with a name and offset into the audio buffer.

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

enum Mark

Constants that describe the type of text.

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
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Supplying metadata

typealias AVSpeechSynthesisProviderOutputBlock

A type that represents the method for sending marker information to the host.

var speechSynthesisOutputMetadataBlock: AVSpeechSynthesisProviderOutputBlock?

A block that subclasses use to send marker information to the host.

