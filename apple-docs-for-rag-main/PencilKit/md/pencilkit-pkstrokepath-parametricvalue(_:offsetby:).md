

- PencilKit
- PKStrokePath
-  parametricValue(\_:offsetBy:) 

Instance Method

# parametricValue(\_:offsetBy:)

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func parametricValue(
    _ parametricValue: CGFloat,
    offsetBy step: PKStrokePath.InterpolatedSlice.Stride
) -> CGFloat
```

## See Also

### Accessing and interpolating points

func interpolatedPoints(in: ClosedRange&lt;CGFloat>?, by: PKStrokePath.InterpolatedSlice.Stride) -> PKStrokePath.InterpolatedSlice

Returns the slice on-curve points using the floating point range and stride that you specify.

func interpolatedLocation(at: CGFloat) -> CGPoint

Returns the on-curve point for the floating point parametric value.

func interpolatedPoint(at: CGFloat) -> PKStrokePoint

Returns the on-curve point for the provided floating point parameter.

