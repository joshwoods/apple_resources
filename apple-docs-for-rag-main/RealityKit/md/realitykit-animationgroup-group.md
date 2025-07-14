

- RealityKit
- AnimationGroup
-  group 

Instance Property

# group

A collection of animations to run.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var group: [any AnimationDefinition] { get set }
```

## See Also

### Configuring the group

var name: String

A textual name for the group.

var bindTarget: BindTarget

A textual name that refers to a property on which to run the grouped animations.

var blendLayer: Int32

The order in which the framework composites the animation.

var additive: Bool

A Boolean value that indicates whether the animation builds on the current state of the target entity or resets the state before running.

var group_: [any AnimationDefinition]?

An optional collection of animations to run.

Deprecated

