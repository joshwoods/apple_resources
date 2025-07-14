

- SpriteKit
- SKInterpolationMode
-  SKInterpolationMode.spline 

Case

# SKInterpolationMode.spline

Values between two keyframes using a spline curve.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case spline
```

## Mentioned in 

Using Keyframe Sequence to effect Custom Interpolation

## Discussion

Given a sequence with the key values of `[5, 1, 10, 0]` and times of `[0, 0.25, 0.5, 1]`, spline interpolation produces a set of values that follow a smooth curve.

## See Also

### Constants

case linear

Values between two keyframes are interpolated linearly.

case step

Values between two keyframes are not interpolated. Instead, the value is that of the most recent keyframe.

