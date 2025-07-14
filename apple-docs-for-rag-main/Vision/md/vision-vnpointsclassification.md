

- Vision
-  VNPointsClassification 

Enumeration

# VNPointsClassification

The set of classifications that describe how to interpret the points the region provides.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
@frozen
enum VNPointsClassification
```

## Topics

### Enumeration Cases

case closedPath

case disconnected

case openPath

### Creating a Classification

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Describing Region Points

var pointsClassification: VNPointsClassification

An enumeration that describes how to interpret the points the region provides.

