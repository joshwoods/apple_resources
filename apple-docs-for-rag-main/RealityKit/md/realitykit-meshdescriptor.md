

- RealityKit
-  MeshDescriptor 

Structure

# MeshDescriptor

Defines a 3D mesh’s structure and data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct MeshDescriptor
```

## Overview

Create or modify 3D shapes in a RealityKit scene using `MeshDescriptor`, which provides properties and methods to define the vertices, normals, texture coordinates, and other attributes of the mesh.

Apply the mesh to an Entity by creating a MeshResource with generate(from:), and create a ModelComponent with init(mesh:materials:).

Start by creating a basic triangle with a `MeshDescriptor` instance.

```
var descriptor = MeshDescriptor(name: "triangle")
descriptor.positions = MeshBuffers.Positions([
    [-1, -1, 0], [1, -1, 0], [0, 1, 0]
])
descriptor.primitives = .triangles([0, 1, 2])
```

## Topics

### Initializers

init(name: String)

Creates an empty mesh descriptor.

### Instance Properties

var buffers: [MeshBuffers.Identifier : AnyMeshBuffer]

Descriptors for the buffers.

var materials: MeshDescriptor.Materials

Material assignments.

var name: String

The name of the mesh.

var primitives: MeshDescriptor.Primitives?

The primitives that make up the mesh.

### Subscripts

subscript&lt;S>(S) -> MeshBuffer&lt;S.Element>?

The buffer for a given semantic. There can only be one buffer for any given ID.

### Enumerations

enum Materials

enum Primitives

Indicates which primitive shape type a mesh applies to its vertex indices.

### Default Implementations

MeshBufferContainer Implementations

## Relationships

### Conforms To

- MeshBufferContainer

## See Also

### Static meshes

enum Primitives

Indicates which primitive shape type a mesh applies to its vertex indices.

enum Materials

