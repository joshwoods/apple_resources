

- RealityKit
- Entity
-  isEnabledInHierarchy 

Instance Property

# isEnabledInHierarchy

A Boolean that indicates whether the entity and all of its ancestors are enabled.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var isEnabledInHierarchy: Bool { get }
```

## Discussion

The value of this property is `true` if the entity and all of its ancestors are enabled, regardless of anchor state.

## See Also

### Managing the entity’s state

var isEnabled: Bool

A Boolean that you set to enable or disable the entity and its descendants.

var isActive: Bool

A Boolean that indicates whether the entity is active.

var isAnchored: Bool

A Boolean that indicates whether the entity is anchored.

