

- Vision
- VNRecognizeTextRequest
-  recognitionLevel 

Instance Property

# recognitionLevel

A value that determines whether the request prioritizes accuracy or speed in text recognition.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var recognitionLevel: VNRequestTextRecognitionLevel { get set }
```

## Mentioned in 

Recognizing Text in Images

## Discussion

The recognition level determines which techniques the request uses during the text recognition. Set this value to VNRequestTextRecognitionLevel.fast to prioritize speed over accuracy, and to VNRequestTextRecognitionLevel.accurate for longer, more computationally intensive recognition.

## See Also

### Customizing Recognition Constraints

var minimumTextHeight: Float

The minimum height, relative to the image height, of the text to recognize.

enum VNRequestTextRecognitionLevel

Constants that identify the performance and accuracy of the text recognition.

