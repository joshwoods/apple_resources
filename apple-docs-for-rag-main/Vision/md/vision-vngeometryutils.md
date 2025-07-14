

- Vision
-  VNGeometryUtils 

Class

# VNGeometryUtils

Utility methods to determine the geometries of various Vision types.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class VNGeometryUtils
```

## Topics

### Calculating Bounding Circles

class func boundingCircle(for: VNContour) throws -> VNCircle

Calculates a bounding circle for the specified contour object.

class func boundingCircle(for: [VNPoint]) throws -> VNCircle

Calculates a bounding circle for the specified array of points.

class func boundingCircle(forSIMDPoints: UnsafePointer&lt;simd_float2>, pointCount: Int) throws -> VNCircle

Calculates a bounding circle for the specified points.

### Calculating Area and Perimeter

class func calculateArea(UnsafeMutablePointer&lt;Double>, for: VNContour, orientedArea: Bool) throws

Calculates the area for the specified contour.

class func calculatePerimeter(UnsafeMutablePointer&lt;Double>, for: VNContour) throws

Calculates the perimeter of a closed contour.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Utilities

struct VNComputeStage

Types that represent the compute stage.

class VNVideoProcessor

An object that performs offline analysis of video content.

