

- RealityKit
- AnimationGroup
-  name 

Instance Property

# name

A textual name for the group.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var name: String { get set }
```

## See Also

### Configuring the group

var group: [any AnimationDefinition]

A collection of animations to run.

var bindTarget: BindTarget

A textual name that refers to a property on which to run the grouped animations.

var blendLayer: Int32

The order in which the framework composites the animation.

var additive: Bool

A Boolean value that indicates whether the animation builds on the current state of the target entity or resets the state before running.

var group_: [any AnimationDefinition]?

An optional collection of animations to run.

Deprecated

