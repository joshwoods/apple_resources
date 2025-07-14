

- SceneKit
-  SCNGeometryTessellator 

Class

# SCNGeometryTessellator

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 12.0+visionOS 1.0+

``` source
class SCNGeometryTessellator
```

## Topics

### Choosing a Smoothing Algorithm

var smoothingMode: SCNTessellationSmoothingMode

enum SCNTessellationSmoothingMode

### Instance Properties

var edgeTessellationFactor: CGFloat

var insideTessellationFactor: CGFloat

var isAdaptive: Bool

var isScreenSpace: Bool

var maximumEdgeLength: CGFloat

var tessellationFactorScale: CGFloat

var tessellationPartitionMode: MTLTessellationPartitionMode

## Relationships

### Inherits From

- NSObject

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

## See Also

### Managing Tessellation

var tessellator: SCNGeometryTessellator?

