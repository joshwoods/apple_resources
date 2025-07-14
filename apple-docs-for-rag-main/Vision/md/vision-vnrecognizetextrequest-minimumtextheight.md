

- Vision
- VNRecognizeTextRequest
-  minimumTextHeight 

Instance Property

# minimumTextHeight

The minimum height, relative to the image height, of the text to recognize.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var minimumTextHeight: Float { get set }
```

## Discussion

Specify a floating-point number relative to the image height. For example, to limit recognition to text that’s half of the image height, use `0.5`. Increasing the size reduces memory consumption and expedites recognition with the tradeoff of ignoring text smaller than the minimum height. The default value is 1/32, or `0.03125`.

## See Also

### Customizing Recognition Constraints

var recognitionLevel: VNRequestTextRecognitionLevel

A value that determines whether the request prioritizes accuracy or speed in text recognition.

enum VNRequestTextRecognitionLevel

Constants that identify the performance and accuracy of the text recognition.

