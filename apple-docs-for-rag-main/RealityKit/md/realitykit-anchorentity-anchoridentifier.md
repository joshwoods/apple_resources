

- RealityKit
- AnchorEntity
-  anchorIdentifier 

Instance Property

# anchorIdentifier

The identifier of the AR anchor with which the anchor entity is associated, or `nil` if it isn’t currently anchored.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var anchorIdentifier: UUID? { get }
```

## See Also

### Configuring the anchor

var anchoring: AnchoringComponent

The component that describes how the virtual content is anchored to the real world.

func reanchor(AnchoringComponent.Target, preservingWorldTransform: Bool)

Changes the entity’s anchoring, preserving either the world transform or the local transform.

