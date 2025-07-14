

- RealityKit
- Anchors
- AnchorEntity
-  HasAnchoring Implementations 

API Collection

# HasAnchoring Implementations

## Topics

### Instance Properties

var anchorIdentifier: UUID?

The identifier of the AR anchor with which the anchor entity is associated, or `nil` if it isn’t currently anchored.

var anchoring: AnchoringComponent

The component that describes how the virtual content is anchored to the real world.

### Instance Methods

func reanchor(AnchoringComponent.Target, preservingWorldTransform: Bool)

Changes the entity’s anchoring, preserving either the world transform or the local transform.

