

- Vision
-  VNRectangleObservation 

Class

# VNRectangleObservation

An object that represents the four vertices of a detected rectangle.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNRectangleObservation
```

## Topics

### Creating an Observation

convenience init(requestRevision: Int, topLeft: CGPoint, topRight: CGPoint, bottomRight: CGPoint, bottomLeft: CGPoint)

Creates a rectangle observation from its corner points.

convenience init(requestRevision: Int, topLeft: CGPoint, bottomLeft: CGPoint, bottomRight: CGPoint, topRight: CGPoint)

Creates a rectangle observation from its corner points.

Deprecated

### Accessing the Coordinates

var bottomLeft: CGPoint

The coordinates of the lower-left corner of the observation bounding box.

var bottomRight: CGPoint

The coordinates of the lower-right corner of the observation bounding box.

var topLeft: CGPoint

The coordinates of the upper-left corner of the observation bounding box.

var topRight: CGPoint

The coordinates of the upper-right corner of the observation bounding box.

## Relationships

### Inherits From

- VNDetectedObjectObservation

### Inherited By

- VNBarcodeObservation
- VNRecognizedTextObservation
- VNTextObservation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- VNRequestRevisionProviding

## See Also

### Accessing the Results

var results: [VNRectangleObservation]?

The results of a document segmentation request.

