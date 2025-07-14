

- UIKit
- UIView
- UIView.KeyframeAnimationOptions
-  calculationModeCubicPaced 

Type Property

# calculationModeCubicPaced

The option to compute intermediate frames using the cubic scheme while ignoring the timing properties of the animation.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
static var calculationModeCubicPaced: UIView.KeyframeAnimationOptions { get }
```

## Discussion

Instead, timing parameters are calculated implicitly to give the animation a constant velocity.

## See Also

### Constants

static var layoutSubviews: UIView.KeyframeAnimationOptions

The option to lay out subviews at commit time so that they’re animated along with their parent.

static var allowUserInteraction: UIView.KeyframeAnimationOptions

The option that allows a person to interact with views while they’re being animated.

static var beginFromCurrentState: UIView.KeyframeAnimationOptions

The option to start an animation from the current setting associated with an already in-flight animation.

static var `repeat`: UIView.KeyframeAnimationOptions

The option to repeat an animation indefinitely.

static var autoreverse: UIView.KeyframeAnimationOptions

The option to run an animation backwards and forwards.

static var overrideInheritedDuration: UIView.KeyframeAnimationOptions

The option to force an animation to use the original duration value specified when the animation was submitted.

static var overrideInheritedOptions: UIView.KeyframeAnimationOptions

The option to not inherit the animation type or any options.

static var calculationModeLinear: UIView.KeyframeAnimationOptions

The option to use a simple linear calculation when interpolating between keyframe values.

static var calculationModeDiscrete: UIView.KeyframeAnimationOptions

The option to not interpolate between keyframe values, but rather to jump directly to each new keyframe value.

static var calculationModePaced: UIView.KeyframeAnimationOptions

The option to compute intermediate keyframe values using a simple pacing algorithm.

static var calculationModeCubic: UIView.KeyframeAnimationOptions

The option to compute intermediate frames using a default Catmull-Rom spline that passes through the keyframe values.

