

- RealityKit
- ModelSortGroupComponent
-  group 

Instance Property

# group

The group that the component’s entity belongs to.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
var group: ModelSortGroup { get set }
```

## Discussion

The renderer only draws entities with the same ModelSortGroup relative to each other.

Note

Membership only applies to the entity that directly owns this component, but not to its descendants.

