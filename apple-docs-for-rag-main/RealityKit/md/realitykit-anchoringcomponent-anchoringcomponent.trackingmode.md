

- RealityKit
- AnchoringComponent
-  AnchoringComponent.TrackingMode 

Structure

# AnchoringComponent.TrackingMode

Decides how the `Entity` tracks its target anchor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct TrackingMode
```

## Topics

### Operators

static func == (AnchoringComponent.TrackingMode, AnchoringComponent.TrackingMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static let continuous: AnchoringComponent.TrackingMode

Continuously anchors the entity to its target based on the target’s realtime location and hides the entity when the target is no longer in frame.

static let once: AnchoringComponent.TrackingMode

Anchors the entity to the target on the first frame the target is found.

static let predicted: AnchoringComponent.TrackingMode

Continuously anchors the entity to its target based on the target’s predicted location and hides the entity when the target is no longer in frame.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Anchoring component

struct AnchoringComponent

A component that anchors virtual content to a real world target.

enum Target

Defines the kinds of real world objects to which an anchor entity can be tethered.

class AnchorEntity

An anchor that tethers entities to a scene.

protocol HasAnchoring

An interface that enables anchoring of virtual content to a real-world object in an AR scene.

