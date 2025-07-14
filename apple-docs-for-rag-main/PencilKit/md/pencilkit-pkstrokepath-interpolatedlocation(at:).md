

- PencilKit
- PKStrokePath
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

A CGPoint interpolated from the supplied `parametricValue`.

## See Also

### Accessing and interpolating points

func interpolatedPoints(in: ClosedRange&lt;CGFloat>?, by: PKStrokePath.InterpolatedSlice.Stride) -> PKStrokePath.InterpolatedSlice

Returns the slice on-curve points using the floating point range and stride that you specify.

func interpolatedPoint(at: CGFloat) -> PKStrokePoint

Returns the on-curve point for the provided floating point parameter.

func parametricValue(CGFloat, offsetBy: PKStrokePath.InterpolatedSlice.Stride) -> CGFloat

