

- RealityKit
- LowLevelMesh
-  LowLevelMesh.Part 

Structure

# LowLevelMesh.Part

An object that describes a range of primitives to display, and their material index.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Part
```

## Topics

### Creating a low-level mesh part

init(indexOffset: Int, indexCount: Int, topology: MTLPrimitiveType, materialIndex: Int, bounds: BoundingBox)

Creates a low-level mesh part.

### Describing a low-level mesh part

var indexOffset: Int

The offset, in bytes, of the first index.

var indexCount: Int

The number of indices to use for this part.

var topology: MTLPrimitiveType

The geometric primitive to use when rendering this part.

var materialIndex: Int

The material index this part associates with.

var bounds: BoundingBox

The model-space bounding box of this part.

## See Also

### Updatable meshes

Creating a spatial drawing app with RealityKit

Use low-level mesh and texture APIs to achieve fast updates to a person’s brush strokes by integrating RealityKit with ARKit and SwiftUI.

Creating a plane with low-level mesh

Create a low-level mesh and set its vertex positions and normals to form a plane.

class LowLevelMesh

A container for vertex data that you can use to create and update meshes using your own format.

struct Descriptor

An object that describes the data format and layout of the buffers in a low-level mesh.

struct Layout

An object that describes a set of attributes that share a buffer index, offset, and stride.

struct Attribute

An object that determines how to store vertex attribute data in memory and map it to RealityKit shader attributes.

enum VertexSemantic

Designates the intended usage of a vertex attribute.

struct PartsCollection

An object that holds a mutable collection low-level mesh parts.

