

- RealityKit
- AnchoringComponent
-  AnchoringComponent.Target 

Enumeration

# AnchoringComponent.Target

Defines the kinds of real world objects to which an anchor entity can be tethered.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+visionOS

``` source
enum Target
```

## Topics

### Basic anchor targets

case world(transform: float4x4)

An anchor point attached to a fixed position in the scene.

case plane(AnchoringComponent.Target.Alignment, classification: AnchoringComponent.Target.Classification, minimumBounds: SIMD2&lt;Float>)

An anchor point attached to a real world surface.

case camera

An anchor point attached to the device’s camera.

case anchor(identifier: UUID)

An anchor point attached to the AR anchor with a given identifier.

### Human anchor targets

case face

An anchor point attached to the user’s face.

case body

An anchor point attached to a human body in motion within the scene.

case hand(AnchoringComponent.Target.Chirality, location: AnchoringComponent.Target.HandLocation)

An anchor point attached to a specific location on the user’s hand.

case head

An anchor point attached to the user’s head.

### Image and object anchor targets

case image(group: String, name: String)

An anchor point attached to the image specified by a group and a name in AR Resources.

case referenceImage(from: AnchoringComponent.ImageAnchoringSource)

An anchor point attached to the image specified by an image anchoring source.

case object(group: String, name: String)

An anchor point attached to the object specified by a group and a name in AR Resources.

case referenceObject(from: AnchoringComponent.ObjectAnchoringSource)

An anchor point attached to the object specified by an object anchoring source.

### Comparing targets

static func == (AnchoringComponent.Target, AnchoringComponent.Target) -> Bool

Indicates whether two targets are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of the target by feeding them into the given hash function.

var hashValue: Int

The hash value.

### Structures

struct Alignment

Defines the alignment of real-world surfaces to seek as targets.

struct Classification

Defines types of real-world surfaces to seek as targets.

struct HandLocation

Defines the locations of tracked hands to look for.

### Enumerations

enum Chirality

Defines the chirality of tracked hands to look for.

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

struct TrackingMode

Decides how the `Entity` tracks its target anchor.

class AnchorEntity

An anchor that tethers entities to a scene.

protocol HasAnchoring

An interface that enables anchoring of virtual content to a real-world object in an AR scene.

