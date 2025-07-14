

- ARKit
-  ARConfidenceLevel 

Enumeration

# ARConfidenceLevel

Degrees to which the framework is confident about depth-data accuracy.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
enum ARConfidenceLevel
```

## Topics

### Levels

case low

Depth-value accuracy in which the framework is less confident.

case medium

Depth-value accuracy in which the framework is moderately confident.

case high

Depth-value accuracy in which the framework is fairly confident.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Comparable
- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Depth Information

var depthMap: CVPixelBuffer

The estimated distance from the device to its environment, in meters.

var confidenceMap: CVPixelBuffer?

The framework’s confidence in the accuracy of the depth-map data.

