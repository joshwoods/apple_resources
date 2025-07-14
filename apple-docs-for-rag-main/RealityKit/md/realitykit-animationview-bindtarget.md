

- RealityKit
- AnimationView
-  bindTarget 

Instance Property

# bindTarget

A textual name that identifies the animated property.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var bindTarget: BindTarget { get set }
```

## Discussion

The property name is a key path. For more information on key paths, see Key-Path Expressions.

## See Also

### Configuring the animation view

var source: (any AnimationDefinition)?

The original animation that this structure modifies.

var name: String

A textual name for the animation.

var blendLayer: Int32

The order in which the framework composites the animation.

