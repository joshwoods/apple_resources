

- SpriteKit
- SKInterpolationMode
-  SKInterpolationMode.step 

Case

# SKInterpolationMode.step

Values between two keyframes are not interpolated. Instead, the value is that of the most recent keyframe.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case step
```

## Discussion

Given a sequence with the key values of `[5, 1, 10, 0]` and times of `[0, 0.25, 0.5, 1]`, step interpolation produces a set of values that follow a series of steps between each keyframe.

## See Also

### Constants

case linear

Values between two keyframes are interpolated linearly.

case spline

Values between two keyframes using a spline curve.

