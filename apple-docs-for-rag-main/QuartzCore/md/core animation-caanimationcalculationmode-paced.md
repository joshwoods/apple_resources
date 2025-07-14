

- Core Animation
- CAAnimationCalculationMode
-  paced 

Type Property

# paced

Linear keyframe values are interpolated to produce an even pace throughout the animation.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
static let paced: CAAnimationCalculationMode
```

## Discussion

`kCAAnimationPaced` gives a linearly interpolated animation, but keyTimes and timingFunction are ignored and keyframe times are automatically generated to give the animation a constant velocity.

The following code shows how to create a keyframe animation object using paced interpolation.

Listing 1. Creating paced key values

```
let keyframeAnimation = CAKeyframeAnimation(keyPath: "position.y")
keyframeAnimation.calculationMode = kCAAnimationPaced
keyframeAnimation.values = [310, 60, 120, 60, 310]
```

A layer animated with the keyframe animation created by the code above and with linearly interpolated horizontal movement would describe a path similar to the following figure.

## See Also

### Constants

static let linear: CAAnimationCalculationMode

Simple linear calculation between keyframe values.

static let discrete: CAAnimationCalculationMode

Each keyframe value is used in turn, no interpolated values are calculated.

static let cubic: CAAnimationCalculationMode

Smooth spline calculation between keyframe values.

static let cubicPaced: CAAnimationCalculationMode

Cubic keyframe values are interpolated to produce an even pace throughout the animation.

