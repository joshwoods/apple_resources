

- ARKit
- MeshAnchor
-  MeshAnchor.MeshClassification 

Enumeration

# MeshAnchor.MeshClassification

The kinds of classification a face of a mesh can have.

visionOS 1.0+

``` source
enum MeshClassification
```

## Topics

### Getting architecture classifications

case ceiling

A ceiling.

case door

A door.

case floor

A floor.

case stairs

A set of stairs.

case wall

A wall.

case window

A window.

### Getting furniture classifications

case bed

A bed.

case cabinet

A cabinet.

case homeAppliance

A home appliance.

case seat

A seat.

case table

A table.

### Getting decoration classifications

case plant

A plant.

case tv

A television.

### Getting unknown classifications

case none

An unknown classification.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting mesh information

var originFromAnchorTransform: simd_float4x4

The location and orientation of a mesh in world space.

var geometry: MeshAnchor.Geometry

The shape of a mesh anchor.

struct Geometry

The shapes that make up a mesh anchor.

