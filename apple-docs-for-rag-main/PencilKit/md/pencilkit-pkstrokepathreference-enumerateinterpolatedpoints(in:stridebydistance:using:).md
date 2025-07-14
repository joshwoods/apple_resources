

- PencilKit
- PKStrokePathReference
-  enumerateInterpolatedPoints(in:strideByDistance:using:) 

Instance Method

# enumerateInterpolatedPoints(in:strideByDistance:using:)

Executes a given block using each point in a range with a distance step.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func enumerateInterpolatedPoints(
    in range: __PKFloatRange,
    strideByDistance distanceStep: CGFloat,
    using block: @escaping (PKStrokePoint, UnsafeMutablePointer) -> Void
)
```

## Parameters 

`range`  

The parametric range to enumerate points in.

`distanceStep`  

The distance to step between points.

`block`  

The block to execute for each point. This block takes two parameters:

- `point` —The interpolated point on the spline.

- `stop` —A reference to a Boolean value. Setting the value to `YES` within the block stops further enumeration, but the that block continues to run until it’s finished.

## See Also

### Accessing and interpolating points

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

