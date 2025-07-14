

- RealityKit
- SampledAnimation
-  bindTarget 

Instance Property

# bindTarget

A textual name that identifies the particular property that animates.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var bindTarget: BindTarget { get set }
```

## Discussion

The property name is a key path. For more information on key paths, see Key-Path Expressions.

## See Also

### Configuring the animation

var name: String

A textual name for the animation.

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

var tweenMode: TweenMode

An option that determines how animation frames transition.

