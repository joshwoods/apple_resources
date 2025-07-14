

- VisionKit
- RecognizedItem
- RecognizedItem.Text
-  observation 

Instance Property

# observation

An object that contains details about the location and content of text and glyphs in an image.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
var observation: VNRecognizedTextObservation { get }
```

## Discussion

Use this property only if you need vision details that aren’t included in the recognized item properties.

## See Also

### Locating text

var bounds: RecognizedItem.Bounds

The bounds of the recognized item in view coordinates.

