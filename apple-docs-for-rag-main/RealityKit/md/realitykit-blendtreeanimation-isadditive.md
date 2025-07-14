

- RealityKit
- BlendTreeAnimation
-  isAdditive 

Instance Property

# isAdditive

A Boolean value that indicates whether the animation builds on the current state of the target entity or resets the state before running.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var isAdditive: Bool { get set }
```

## See Also

### Configuring the animation

var root: any BlendTreeNode

The first node in a tree of animations.

var name: String

A textual name for the animation.

var bindTarget: BindTarget

A textual name that identifies the particular property that animates.

var blendLayer: Int32

The order in which the framework composites the animation.

