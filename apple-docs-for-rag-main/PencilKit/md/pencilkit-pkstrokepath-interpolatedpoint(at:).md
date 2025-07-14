

- PencilKit
- PKStrokePath
-  interpolatedPoint(at:) 

Instance Method

# interpolatedPoint(at:)

Returns the on-curve point for the provided floating point parameter.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func interpolatedPoint(at parametricValue: CGFloat) -> PKStrokePoint
```

## Parameters 

`parametricValue`  

The on-curve location `[0, count-1]` where interpolation occurs.

## Return Value

A PKStrokePoint interpolated from the supplied `parametricValue.`

## See Also

### Accessing and interpolating points

func interpolatedPoints(in: ClosedRange&lt;CGFloat>?, by: PKStrokePath.InterpolatedSlice.Stride) -> PKStrokePath.InterpolatedSlice

Returns the slice on-curve points using the floating point range and stride that you specify.

func interpolatedLocation(at: CGFloat) -> CGPoint

Returns the on-curve point for the floating point parametric value.

func parametricValue(CGFloat, offsetBy: PKStrokePath.InterpolatedSlice.Stride) -> CGFloat

