

- RealityKit
- FromToByAnimation
-  jointNames 

Instance Property

# jointNames

Joint names that define the joints in the skeletal pose.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var jointNames: [String] { get set }
```

Available when `Value` is `JointTransforms`.

## See Also

### Configuring the animation

var name: String

A textual name for the animation.

var bindTarget: BindTarget

A textual name that identifies the particular property that animates.

var blendLayer: Int32

The order in which the framework composites the animation.

var isScaleAnimated: Bool

A Boolean value that indicates whether that animation interpolates changes to the target’s size.

var isRotationAnimated: Bool

A Boolean value that indicates whether the animation interpolates rotational changes.

var isTranslationAnimated: Bool

A Boolean value that indicates whether the animation interpolates changes to the target object’s position.

var isAdditive: Bool

A Boolean value that indicates whether the animation blends additively with concurrent animations.

