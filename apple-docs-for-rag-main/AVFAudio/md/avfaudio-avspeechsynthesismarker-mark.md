

- AVFAudio
- AVSpeechSynthesisMarker
-  mark 

Instance Property

# mark

The type that describes the text.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var mark: AVSpeechSynthesisMarker.Mark { get set }
```

## See Also

### Inspecting a marker

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

