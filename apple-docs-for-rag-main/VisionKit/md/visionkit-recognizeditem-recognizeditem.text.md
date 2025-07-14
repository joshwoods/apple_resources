

- VisionKit
- RecognizedItem
-  RecognizedItem.Text 

Structure

# RecognizedItem.Text

An object that represents a text item that the scanner recognizes.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
struct Text
```

## Topics

### Getting text strings

var transcript: String

The string that the text item represents.

### Locating text

var bounds: RecognizedItem.Bounds

The bounds of the recognized item in view coordinates.

var observation: VNRecognizedTextObservation

An object that contains details about the location and content of text and glyphs in an image.

### Identifying text

var id: UUID

A unique identifier for the recognized item.

## Relationships

### Conforms To

- Identifiable

## See Also

### Text items

case text(RecognizedItem.Text)

Text or data the analyzer detects in text.

