

- SpriteKit
- SKInterpolationMode
-  SKInterpolationMode.linear 

Case

# SKInterpolationMode.linear

Values between two keyframes are interpolated linearly.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case linear
```

## Discussion

Given a sequence with the key values of `[5, 1, 10, 0]` and times of `[0, 0.25, 0.5, 1]`, linear interpolation produces a set of values that follow a series of straight lines between each keyframe.

## See Also

### Constants

case spline

Values between two keyframes using a spline curve.

case step

Values between two keyframes are not interpolated. Instead, the value is that of the most recent keyframe.

