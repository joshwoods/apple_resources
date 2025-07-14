

- RealityKit
- LowLevelMesh
-  LowLevelMesh.Descriptor 

Structure

# LowLevelMesh.Descriptor

An object that describes the data format and layout of the buffers in a low-level mesh.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Descriptor
```

## Topics

### Creating a low-level mesh descriptor

init(vertexCapacity: Int, vertexAttributes: [LowLevelMesh.Attribute], vertexLayouts: [LowLevelMesh.Layout], indexCapacity: Int, indexType: MTLIndexType)

Creates a descriptor for a low-level mesh.

### Defining the descriptor’s contents

var indexType: MTLIndexType

The data type of the indices that the index buffer stores.

var vertexAttributes: [LowLevelMesh.Attribute]

An array that describes the vertex input attributes to a vertex function.

var vertexLayouts: [LowLevelMesh.Layout]

The list of layouts.

var vertexBufferCount: Int

The number of buffers this descriptor uses.

### Defining the descriptor’s limits

var vertexCapacity: Int

The number of vertices to allocate space for.

var indexCapacity: Int

The number of indices to allocate space for.

static let maxVertexBufferCount: Int

The maximum number of separate buffers the system supports.

## See Also

### Updatable meshes

Creating a spatial drawing app with RealityKit

Use low-level mesh and texture APIs to achieve fast updates to a person’s brush strokes by integrating RealityKit with ARKit and SwiftUI.

Creating a plane with low-level mesh

Create a low-level mesh and set its vertex positions and normals to form a plane.

class LowLevelMesh

A container for vertex data that you can use to create and update meshes using your own format.

struct Part

An object that describes a range of primitives to display, and their material index.

struct Layout

An object that describes a set of attributes that share a buffer index, offset, and stride.

struct Attribute

An object that determines how to store vertex attribute data in memory and map it to RealityKit shader attributes.

enum VertexSemantic

Designates the intended usage of a vertex attribute.

struct PartsCollection

An object that holds a mutable collection low-level mesh parts.

