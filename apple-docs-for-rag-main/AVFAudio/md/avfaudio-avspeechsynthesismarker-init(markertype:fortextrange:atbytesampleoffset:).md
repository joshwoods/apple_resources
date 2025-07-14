

- AVFAudio
- AVSpeechSynthesisMarker
-  init(markerType:forTextRange:atByteSampleOffset:) 

Initializer

# init(markerType:forTextRange:atByteSampleOffset:)

Creates a marker with a type and location of the request’s text.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    markerType type: AVSpeechSynthesisMarker.Mark,
    forTextRange range: NSRange,
    atByteSampleOffset byteSampleOffset: Int
)
```

## Parameters 

`type`  

The type that describes the text.

`range`  

The location and length of the request’s text.

`byteSampleOffset`  

The byte offset into the audio buffer.

## See Also

### Creating a marker

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

