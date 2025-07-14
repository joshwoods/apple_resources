

- RealityKit
- SampledAnimation
-  tweenMode 

Instance Property

# tweenMode

An option that determines how animation frames transition.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var tweenMode: TweenMode { get set }
```

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

var isRotationAnimated: Bool

A Boolean value that indicates whether the animation observes rotational changes in the entity’s transform.

var isScaleAnimated: Bool

A Boolean value that indicates whether the animation observes changes in the entity’s size.

var isTranslationAnimated: Bool

A Boolean value that indicates whether the animation observes translational changes in the entity’s transform.

var additive: Bool

A Boolean value that indicates whether the animation builds on the current state of the target entity or resets the state before running.

