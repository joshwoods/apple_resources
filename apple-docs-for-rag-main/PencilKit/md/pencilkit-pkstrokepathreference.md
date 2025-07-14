

- PencilKit
-  PKStrokePathReference 

Class

# PKStrokePathReference

A class that captures the components of a stroke and provides methods to find and interpolate points along the stroke’s path.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
class PKStrokePathReference
```

## Topics

### Creating a new stroke path

init(controlPoints: [PKStrokePoint], creationDate: Date)

Creates a stroke path with the cubic B-spline control points and a date that you specify.

### Getting the stroke path properties

var count: Int

The number of control points in this stroke path.

var creationDate: Date

The time at which this stroke path starts.

### Accessing and interpolating points

func enumerateInterpolatedPoints(in: __PKFloatRange, strideByDistance: CGFloat, using: (PKStrokePoint, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given block using each point in a range with a distance step.

func enumerateInterpolatedPoints(in: __PKFloatRange, strideByParametricStep: CGFloat, using: (PKStrokePoint, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given block using each point in a range with a parametric step.

func enumerateInterpolatedPoints(in: __PKFloatRange, strideByTime: TimeInterval, using: (PKStrokePoint, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given block using each point in a range with a time step.

func interpolatedLocation(at: CGFloat) -> CGPoint

Returns the on-curve point for the floating point parametric value.

func interpolatedPoint(at: CGFloat) -> PKStrokePoint

Returns the on-curve point for the provided floating point parameter.

func parametricValue(CGFloat, offsetByDistance: CGFloat) -> CGFloat

Returns a parametric value on the B-spline that’s a specified distance from the given parametric value.

func parametricValue(CGFloat, offsetByTime: TimeInterval) -> CGFloat

Returns a parametric value on the B-spline that’s a specified time from the given parametric value.

func point(at: Int) -> PKStrokePoint

Returns the B-spline control point at an index point that you provide.

subscript(Int) -> PKStrokePoint

Returns the B-spline control point the location index that you provide.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

