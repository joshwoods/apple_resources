

- SpriteKit
- SKRepeatMode
-  SKRepeatMode.loop 

Case

# SKRepeatMode.loop

When a sample is calculated, the sequence loops back to the beginning of the sequence. For example, if the last keyframe’s time value is `0.5`, then a sample at any time value from `0.5` to `1.0` returns the same value as the sequence did from `0.0` to `0.5`.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case loop
```

## Discussion

Given a sequence with the key values of `[5, 1, 10]` and times of `[0, 0.25, 0.5]`, loop repeat mode produces a set of values that repeats the previous keyframes when the sample time is `0.5`:

## See Also

### Constants

case clamp

When a sample is calculated, the time value is clamped to the range of time values found in the sequence. For example, if the last keyframe’s time value is `0.5`, a sample at any time value from `0.5` to `1.0` returns the last keyframe’s value.

