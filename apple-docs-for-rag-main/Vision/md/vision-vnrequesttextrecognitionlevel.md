

- Vision
-  VNRequestTextRecognitionLevel 

Enumeration

# VNRequestTextRecognitionLevel

Constants that identify the performance and accuracy of the text recognition.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
enum VNRequestTextRecognitionLevel
```

## Topics

### Recognition Levels

case fast

Fast text recognition returns results more quickly at the expense of accuracy.

case accurate

Accurate text recognition takes more time to produce a more comprehensive result.

### Creating a Recognition Level

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Customizing Recognition Constraints

var minimumTextHeight: Float

The minimum height, relative to the image height, of the text to recognize.

var recognitionLevel: VNRequestTextRecognitionLevel

A value that determines whether the request prioritizes accuracy or speed in text recognition.

