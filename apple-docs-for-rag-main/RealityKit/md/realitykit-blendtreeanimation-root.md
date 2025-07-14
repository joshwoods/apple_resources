

- RealityKit
- BlendTreeAnimation
-  root 

Instance Property

# root

The first node in a tree of animations.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var root: any BlendTreeNode { get set }
```

## Discussion

This property defines the node that represents the root of a blend tree. If you assign this property a BlendTreeBlendNode instance, the root branches for every member you add to the instance’s sources property.

If you define a BlendTreeSourceNode instance to this property, the tree contains a single animation, which blends with no other animations.

## See Also

### Configuring the animation

var name: String

A textual name for the animation.

var bindTarget: BindTarget

A textual name that identifies the particular property that animates.

var blendLayer: Int32

The order in which the framework composites the animation.

var isAdditive: Bool

A Boolean value that indicates whether the animation builds on the current state of the target entity or resets the state before running.

