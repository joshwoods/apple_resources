

- Create ML Components
-  DetectedObject 

Structure

# DetectedObject

An item in a detection result.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct DetectedObject where Label : Comparable, Label : Hashable
```

## Topics

### Creating a detected object

init(boundingBox: CGRect, label: Label, probability: Float)

Creates a detected object with bounding box, object label and confidence.

### Getting the properties

var boundingBox: CGRect

The bounding box of the detected object.

var confidence: Float

The detection confidence. The value will always be between 0.0 and 1.0.

var label: Label

The detected object label.

### Operators

static func == (DetectedObject&lt;Label>, DetectedObject&lt;Label>) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Sendable

## See Also

### Object detection components

struct ObjectDetectionAnnotation

An object detection annotation.

struct ObjectDetectionMetrics

Metrics for object detection model.

