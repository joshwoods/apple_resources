

- Speech
- SFTranscriptionSegment
-  substringRange 

Instance Property

# substringRange

The range information for the transcription segment’s substring, relative to the overall transcription.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var substringRange: NSRange { get }
```

## Discussion

Use the range information to find the position of the segment within the formattedString property of the SFTranscription object containing this segment.

## See Also

### Transcribing the Segment

var substring: String

The string representation of the utterance in the transcription segment.

var alternativeSubstrings: [String]

An array of alternate interpretations of the utterance in the transcription segment.

