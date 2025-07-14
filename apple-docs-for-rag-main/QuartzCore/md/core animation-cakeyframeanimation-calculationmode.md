

- Core Animation
- CAKeyframeAnimation
-  calculationMode 

Instance Property

# calculationMode

Specifies how intermediate keyframe values are calculated by the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var calculationMode: CAAnimationCalculationMode { get set }
```

## Discussion

The possible values are described in Value calculation modes. The default value of this property is linear.

## See Also

### Keyframe timing

var keyTimes: [NSNumber]?

An optional array of `NSNumber` objects that define the time at which to apply a given keyframe segment.

var timingFunctions: [CAMediaTimingFunction]?

An optional array of `CAMediaTimingFunction` objects that define the pacing for each keyframe segment.

