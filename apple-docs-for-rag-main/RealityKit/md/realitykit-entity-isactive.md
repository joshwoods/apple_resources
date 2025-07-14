

- RealityKit
- Entity
-  isActive 

Instance Property

# isActive

A Boolean that indicates whether the entity is active.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var isActive: Bool { get }
```

## Discussion

The value of this property is `true` if the entity is anchored in a scene, and it and all of its ancestors are enabled (isEnabled is set to `true`). RealityKit doesn’t simulate or render inactive entities.

## See Also

### Managing the entity’s state

var isEnabled: Bool

A Boolean that you set to enable or disable the entity and its descendants.

var isEnabledInHierarchy: Bool

A Boolean that indicates whether the entity and all of its ancestors are enabled.

var isAnchored: Bool

A Boolean that indicates whether the entity is anchored.

