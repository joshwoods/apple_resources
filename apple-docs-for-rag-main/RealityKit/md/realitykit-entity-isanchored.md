

- RealityKit
- Entity
-  isAnchored 

Instance Property

# isAnchored

A Boolean that indicates whether the entity is anchored.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var isAnchored: Bool { get }
```

## Discussion

The value of this property is `true` if the entity is anchored in a scene. An entity that isn’t anchored becomes inactive (isActive returns `false`), meaning RealityKit doesn’t render or simulate it.

## See Also

### Managing the entity’s state

var isEnabled: Bool

A Boolean that you set to enable or disable the entity and its descendants.

var isEnabledInHierarchy: Bool

A Boolean that indicates whether the entity and all of its ancestors are enabled.

var isActive: Bool

A Boolean that indicates whether the entity is active.

