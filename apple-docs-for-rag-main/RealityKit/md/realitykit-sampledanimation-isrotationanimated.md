

- RealityKit
- SampledAnimation
-  isRotationAnimated 

Instance Property

# isRotationAnimated

A Boolean value that indicates whether the animation observes rotational changes in the entity’s transform.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var isRotationAnimated: Bool { get set }
```

Available when `Value` is `JointTransforms`.

## Discussion

If you set this property to `true`, the animation accommodates rotational differences in the entity’s transform by interpolating to the target rotation across the animation timeline.

## See Also

### Configuring the animation

var name: String

A textual name for the animation.

var bindTarget: BindTarget

A textual name that identifies the particular property that animates.

var blendLayer: Int32

The order in which the framework composites the animation.

var jointNames: [String]

The names of the joints to animate.

var isScaleAnimated: Bool

A Boolean value that indicates whether the animation observes changes in the entity’s size.

var isTranslationAnimated: Bool

A Boolean value that indicates whether the animation observes translational changes in the entity’s transform.

var additive: Bool

A Boolean value that indicates whether the animation builds on the current state of the target entity or resets the state before running.

var tweenMode: TweenMode

An option that determines how animation frames transition.

