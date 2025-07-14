

- AVFAudio
- AVSpeechSynthesisMarker
-  bookmarkName 

Instance Property

# bookmarkName

A string that represents the name of a bookmark.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var bookmarkName: String { get set }
```

## See Also

### Inspecting a marker

var mark: AVSpeechSynthesisMarker.Mark

The type that describes the text.

var phoneme: String

A string that represents a distinct sound.

var textRange: NSRange

The location and length of the request’s text.

var byteSampleOffset: Int

The byte offset into the audio buffer.

enum Mark

Constants that describe the type of text.

