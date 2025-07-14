

- Vision
-  RecognizedText 

Structure

# RecognizedText

Text recognized in an image through a text recognition request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct RecognizedText
```

## Topics

### Getting the bounding box

func boundingBox(for: Range&lt;String.Index>) -> RectangleObservation?

Calculates the bounding box around the characters in the range of a string.

### Inspecting the recognized text

var string: String

The top candidate for recognized text.

var confidence: Float

A normalized confidence score for the text recognition result.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Getting the recognized text

func topCandidates(Int) -> [RecognizedText]

Requests the top candidates for a recognized text string.

