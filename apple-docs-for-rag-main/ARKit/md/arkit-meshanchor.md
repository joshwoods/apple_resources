

- ARKit
-  MeshAnchor 

Structure

# MeshAnchor

A volume of space that contains a mesh of a person’s surroundings.

visionOS 1.0+

``` source
struct MeshAnchor
```

## Topics

### Getting mesh information

var originFromAnchorTransform: simd_float4x4

The location and orientation of a mesh in world space.

var geometry: MeshAnchor.Geometry

The shape of a mesh anchor.

struct Geometry

The shapes that make up a mesh anchor.

enum MeshClassification

The kinds of classification a face of a mesh can have.

### Inspecting mesh anchors

var id: UUID

The unique identifier of this anchor.

var description: String

A textual representation of this anchor.

## Relationships

### Conforms To

- Anchor
- Copyable
- CustomStringConvertible
- Equatable
- Identifiable
- Sendable

## See Also

### Scene reconstruction

Incorporating real-world surroundings in an immersive experience

Create an immersive experience by making your app’s content respond to the local shape of the world.

class SceneReconstructionProvider

A source of live data about the shape of a person’s surroundings.

