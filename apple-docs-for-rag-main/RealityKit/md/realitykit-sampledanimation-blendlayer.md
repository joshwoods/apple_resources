

- RealityKit
- SampledAnimation
-  blendLayer 

Instance Property

# blendLayer

The order in which the framework composites the animation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var blendLayer: Int32 { get set }
```

## Discussion

The framework applies multiple animations on the same target in ascending order of this property’s value. Animations in a lower layer run before animations in a higher layer. Animations that share the same value apply in the order that they execute.

## See Also

### Configuring the animation

var name: String

A textual name for the animation.

var bindTarget: BindTarget

A textual name that identifies the particular property that animates.

var jointNames: [String]

The names of the joints to animate.

var isRotationAnimated: Bool

A Boolean value that indicates whether the animation observes rotational changes in the entity’s transform.

var isScaleAnimated: Bool

A Boolean value that indicates whether the animation observes changes in the entity’s size.

var isTranslationAnimated: Bool

A Boolean value that indicates whether the animation observes translational changes in the entity’s transform.

var additive: Bool

A Boolean value that indicates whether the animation builds on the current state of the target entity or resets the state before running.

var tweenMode: TweenMode

An option that determines how animation frames transition.

