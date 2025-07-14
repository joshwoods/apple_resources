

- PencilKit
- PKStrokePath
-  interpolatedPoints(in:by:) 

Instance Method

# interpolatedPoints(in:by:)

Returns the slice on-curve points using the floating point range and stride that you specify.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func interpolatedPoints(
    in range: ClosedRange? = nil,
    by stride: PKStrokePath.InterpolatedSlice.Stride
) -> PKStrokePath.InterpolatedSlice
```

## Parameters 

`range`  

The floating point range for the points of interest.

`stride`  

The stride component of the current slice.

## Return Value

An interpolated slice whose points are within the specified `range`.

## See Also

### Accessing and interpolating points

func interpolatedLocation(at: CGFloat) -> CGPoint

Returns the on-curve point for the floating point parametric value.

func interpolatedPoint(at: CGFloat) -> PKStrokePoint

Returns the on-curve point for the provided floating point parameter.

func parametricValue(CGFloat, offsetBy: PKStrokePath.InterpolatedSlice.Stride) -> CGFloat

