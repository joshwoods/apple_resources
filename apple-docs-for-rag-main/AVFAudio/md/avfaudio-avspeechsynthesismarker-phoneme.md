

- AVFAudio
- AVSpeechSynthesisMarker
-  phoneme 

Instance Property

# phoneme

A string that represents a distinct sound.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var phoneme: String { get set }
```

## See Also

### Inspecting a marker

var mark: AVSpeechSynthesisMarker.Mark

The type that describes the text.

var bookmarkName: String

A string that represents the name of a bookmark.

var textRange: NSRange

The location and length of the request’s text.

var byteSampleOffset: Int

The byte offset into the audio buffer.

enum Mark

Constants that describe the type of text.

