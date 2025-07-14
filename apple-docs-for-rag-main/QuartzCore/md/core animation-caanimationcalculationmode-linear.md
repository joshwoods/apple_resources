

- Core Animation
- CAAnimationCalculationMode
-  linear 

Type Property

# linear

Simple linear calculation between keyframe values.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
static let linear: CAAnimationCalculationMode
```

## Discussion

The following code shows how to create a keyframe animation object using linear interpolation.

Listing 1. Creating linearly interpolated keyframes

```
let keyframeAnimation = CAKeyframeAnimation(keyPath: "position.y")
keyframeAnimation.calculationMode = kCAAnimationLinear
keyframeAnimation.keyTimes = [0, 0.25, 0.5, 0.75, 1]
keyframeAnimation.values = [310, 60, 120, 60, 310]
```

A layer animated with the keyframe animation created by the code above and with linearly interpolated horizontal movement would describe a path similar to the following figure.

## See Also

### Constants

static let discrete: CAAnimationCalculationMode

Each keyframe value is used in turn, no interpolated values are calculated.

static let paced: CAAnimationCalculationMode

Linear keyframe values are interpolated to produce an even pace throughout the animation.

static let cubic: CAAnimationCalculationMode

Smooth spline calculation between keyframe values.

static let cubicPaced: CAAnimationCalculationMode

Cubic keyframe values are interpolated to produce an even pace throughout the animation.

