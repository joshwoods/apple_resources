

- RealityKit
- Entity
-  isEnabled 

Instance Property

# isEnabled

A Boolean that you set to enable or disable the entity and its descendants.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var isEnabled: Bool { get set }
```

## Mentioned in 

Manipulating Reality Composer scenes from code

## Discussion

Set this value to `true` to enable the entity. Unless an ancestor is disabled, the entity and all of its enabled descendants, up to the first that’s disabled, report isEnabledInHierarchy of `true`. If an ancestor is disabled, they all report `false`. The state of isActive for enabled entities is `true` if they are anchored, or `false` otherwise.

If you disable an entity, it and all of its descendants become both disabled (isEnabledInHierarchy returns `false`) and inactive (isActive returns `false`), regardless of any other state.

When an entity is disabled, it’s no longer visible in your scene. However, the entity is still included in an EntityQuery.

## See Also

### Managing the entity’s state

var isEnabledInHierarchy: Bool

A Boolean that indicates whether the entity and all of its ancestors are enabled.

var isActive: Bool

A Boolean that indicates whether the entity is active.

var isAnchored: Bool

A Boolean that indicates whether the entity is anchored.

