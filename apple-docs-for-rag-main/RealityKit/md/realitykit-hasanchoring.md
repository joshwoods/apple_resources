

- RealityKit
-  HasAnchoring 

Protocol

# HasAnchoring

An interface that enables anchoring of virtual content to a real-world object in an AR scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
protocol HasAnchoring : Entity
```

## Topics

### Getting the component

var anchoring: AnchoringComponent

The component that describes how the virtual content is anchored to the real world.

### Identifying the AR anchor

var anchorIdentifier: UUID?

The identifier of the AR anchor with which the anchor entity is associated, or `nil` if it isn’t currently anchored.

### Moving the anchor

func reanchor(AnchoringComponent.Target, preservingWorldTransform: Bool)

Changes the entity’s anchoring, preserving either the world transform or the local transform.

## Relationships

### Inherits From

- Entity

### Conforming Types

- AnchorEntity

## See Also

### Anchoring component

struct AnchoringComponent

A component that anchors virtual content to a real world target.

enum Target

Defines the kinds of real world objects to which an anchor entity can be tethered.

struct TrackingMode

Decides how the `Entity` tracks its target anchor.

class AnchorEntity

An anchor that tethers entities to a scene.

