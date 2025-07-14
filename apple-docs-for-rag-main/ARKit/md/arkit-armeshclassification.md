

- ARKit
-  ARMeshClassification 

Enumeration

# ARMeshClassification

Enumeration of different classes of real-world objects that ARKit can identify.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
enum ARMeshClassification
```

## Overview

When you enable sceneReconstruction on a world-tracking configuration, ARKit provides several mesh anchors (ARMeshAnchor) that collectively estimate the shape of the physical environment. Within that model of the real world, ARKit may identify specific objects, like seats, windows, tables, or walls. ARKit shares that information by exposing one or more ARMeshClassification instances in a mesh’s geometry property.

For a sample app that demonstrates mesh classification, see Visualizing and interacting with a reconstructed scene.

## Topics

### Options

case ceiling

The face is a part of a real-world ceiling.

case door

The face is a part of a real-world door.

case floor

The face is a part of a real-world floor.

case none

A face ARKit can’t classify.

case seat

The face is a part of a real-world seat.

case table

The face is a part of a real-world table.

case wall

The face is a part of a real-world wall.

case window

The face is a part of a real-world window.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting Geometry Information

var classification: ARGeometrySource?

Classification for each face in the mesh.

var faces: ARGeometryElement

An object that contains a buffer of vertex indices of the geometry’s faces.

class ARGeometryElement

A container for index data, such as vertex indices of a face.

var normals: ARGeometrySource

Rays that define which direction is outside for each face.

