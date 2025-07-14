

- Core Animation
- CAAnimationCalculationMode
-  cubic 

Type Property

# cubic

Smooth spline calculation between keyframe values.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
static let cubic: CAAnimationCalculationMode
```

## Discussion

Intermediate frames are computed using a Catmull-Rom spline that passes through the keyframes. You can adjust the shape of the spline by specifying an optional set of tension, continuity, and bias values, which modify the spline using the standard Kochanek-Bartels form.

The following code shows how to create a keyframe animation object using cubic interpolation.

```
let keyframeAnimation = CAKeyframeAnimation(keyPath: "position.y")
keyframeAnimation.calculationMode = kCAAnimationCubic
keyframeAnimation.keyTimes = [0, 0.25, 0.5, 0.75, 1]
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

static let cubicPaced: CAAnimationCalculationMode

Cubic keyframe values are interpolated to produce an even pace throughout the animation.

