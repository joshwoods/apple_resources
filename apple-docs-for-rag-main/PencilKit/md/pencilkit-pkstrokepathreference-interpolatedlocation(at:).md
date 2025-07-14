

- PencilKit
- PKStrokePathReference
-  interpolatedLocation(at:) 

Instance Method

# interpolatedLocation(at:)

Returns the on-curve point for the floating point parametric value.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func interpolatedLocation(at parametricValue: CGFloat) -> CGPoint
```

## Parameters 

`parametricValue`  

The on-curve location `[0, count-1]` where interpolation occurs.

## Return Value

A CGPoint interpolated from supplied `parametricValue`.

## See Also

### Accessing and interpolating points

func enumerateInterpolatedPoints(in: __PKFloatRange, strideByDistance: CGFloat, using: (PKStrokePoint, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given block using each point in a range with a distance step.

func enumerateInterpolatedPoints(in: __PKFloatRange, strideByParametricStep: CGFloat, using: (PKStrokePoint, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given block using each point in a range with a parametric step.

func enumerateInterpolatedPoints(in: __PKFloatRange, strideByTime: TimeInterval, using: (PKStrokePoint, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given block using each point in a range with a time step.

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

