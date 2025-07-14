

- AVFAudio
- AVSpeechSynthesisMarker
-  textRange 

Instance Property

# textRange

The location and length of the request’s text.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var textRange: NSRange { get set }
```

## See Also

### Inspecting a marker

var mark: AVSpeechSynthesisMarker.Mark

The type that describes the text.

var bookmarkName: String

A string that represents the name of a bookmark.

var phoneme: String

A string that represents a distinct sound.

var byteSampleOffset: Int

The byte offset into the audio buffer.

enum Mark

Constants that describe the type of text.

