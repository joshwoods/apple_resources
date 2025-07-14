

- Vision
- VNRecognizedText
-  confidence 

Instance Property

# confidence

A normalized confidence score for the text recognition result.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var confidence: VNConfidence { get }
```

## Discussion

The confidence level is a normalized value between `0.0` and `1.0`, where `1.0` represents the highest confidence.

## See Also

### Determining Recognized Text

var string: String

The top candidate for recognized text.

