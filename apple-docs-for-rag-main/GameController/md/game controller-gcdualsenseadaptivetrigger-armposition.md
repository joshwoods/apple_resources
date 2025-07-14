

- Game Controller
- GCDualSenseAdaptiveTrigger
-  armPosition 

Instance Property

# armPosition

The position of the trigger’s arm.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+

``` source
var armPosition: Float { get }
```

## Discussion

This property represents the value of the stepped mechanical arm inside the trigger and isn’t the same as the trigger’s inherited `value` property. This property ranges between `0` and `1`, where `0` represents the minimum and `1` represents the maximum position.

## See Also

### Getting the arm position

class var discretePositionCount: Int

The number of discrete control positions that the DualSense adaptive triggers support.

