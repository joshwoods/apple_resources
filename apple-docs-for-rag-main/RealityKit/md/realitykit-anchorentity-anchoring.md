

- RealityKit
- AnchorEntity
-  anchoring 

Instance Property

# anchoring

The component that describes how the virtual content is anchored to the real world.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var anchoring: AnchoringComponent { get set }
```

## See Also

### Configuring the anchor

var anchorIdentifier: UUID?

The identifier of the AR anchor with which the anchor entity is associated, or `nil` if it isn’t currently anchored.

func reanchor(AnchoringComponent.Target, preservingWorldTransform: Bool)

Changes the entity’s anchoring, preserving either the world transform or the local transform.

