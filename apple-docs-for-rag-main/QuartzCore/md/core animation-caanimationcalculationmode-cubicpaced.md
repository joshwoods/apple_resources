

- Core Animation
- CAAnimationCalculationMode
-  cubicPaced 

Type Property

# cubicPaced

Cubic keyframe values are interpolated to produce an even pace throughout the animation.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
static let cubicPaced: CAAnimationCalculationMode
```

## Discussion

`kCAAnimationCubicPaced` gives a linearly interpolated animation, but keyTimes and timingFunction are ignored and keyframe times are automatically generated to give the animation a constant velocity.

The following code shows how to create a keyframe animation object using paced cubic interpolation.

```
let keyframeAnimation = CAKeyframeAnimation(keyPath: "position.y")
keyframeAnimation.calculationMode = kCAAnimationCubicPaced
keyframeAnimation.values = [310, 60, 120, 60, 310]
```

A layer animated with the keyframe animation created by the code above and with linearly interpolated horizontal movement would describe a path similar to the following figure.

## See Also

### Constants

static let linear: CAAnimationCalculationMode

Simple linear calculation between keyframe values.

static let discrete: CAAnimationCalculationMode

Each keyframe value is used in turn, no interpolated values are calculated.

static let paced: CAAnimationCalculationMode

Linear keyframe values are interpolated to produce an even pace throughout the animation.

static let cubic: CAAnimationCalculationMode

Smooth spline calculation between keyframe values.

