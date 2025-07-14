

- VisionKit
- RecognizedItem
-  RecognizedItem.Bounds 

Structure

# RecognizedItem.Bounds

An object that represents the four corners of a recognized item.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
struct Bounds
```

## Topics

### Getting the corners of items

var topLeft: CGPoint

The upper-left corner of the recognized item in view coordinates.

var topRight: CGPoint

The upper-right corner of the recognized item in view coordinates.

var bottomRight: CGPoint

The lower-right corner of the recognized item in view coordinates.

var bottomLeft: CGPoint

The lower-left corner of the recognized item in view coordinates.

## Relationships

### Conforms To

- Sendable

## See Also

### Item location

var bounds: RecognizedItem.Bounds

The four corners of the recognized item in view coordinates.

