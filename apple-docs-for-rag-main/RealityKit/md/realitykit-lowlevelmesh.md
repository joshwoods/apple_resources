

- RealityKit
-  LowLevelMesh 

Class

# LowLevelMesh

A container for vertex data that you can use to create and update meshes using your own format.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
class LowLevelMesh
```

## Mentioned in 

Creating a plane with low-level mesh

## Overview

Use `LowLevelMesh` when you want to bring your own vertex format to RealityKit or update your data frequently. To update your data in `LowLevelMesh`, you can either use Swift for CPU processing, or Metal Compute Shaders for GPU processing.

Note

Use MeshDescriptor for a simpler alternative to `LowLevelMesh`. For information on loading a model from a USD or Reality file, see Loading entities from a file.

Express your vertex by creating a LowLevelMesh.Descriptor that describes your layout, along with the required index and vertex capacities. This descriptor is similar to MTLVertexDescriptor, with additional semantics that make the data available in your shaders.

To use `LowLevelMesh`, first define your own vertex structure, either in a Metal header or using a Swift structure:

```
struct MyVertex {
    var position: SIMD3 = .zero
    var color: UInt32 = .zero
}
```

Next, describe your structure to `LowLevelMesh` by creating a list of vertex attributes and a vertex layout. This description informs `LowLevelMesh` how to represent the vertex data in memory:

```
extension MyVertex {
    static var vertexAttributes: [LowLevelMesh.Attribute] = [
        .init(semantic: .position, format: .float3, offset: MemoryLayout.offset(of: \.position)!),
        .init(semantic: .color, format: .uchar4Normalized_bgra, offset: MemoryLayout.offset(of: \.color)!)
    ]

    static var vertexLayouts: [LowLevelMesh.Layout] = [
        .init(bufferIndex: 0, bufferStride: MemoryLayout.stride)
    ]

    static var descriptor: LowLevelMesh.Descriptor {
        var desc = LowLevelMesh.Descriptor()
        desc.vertexAttributes = MyVertex.vertexAttributes
        desc.vertexLayouts = MyVertex.vertexLayouts
        desc.indexType = .uint32
        return desc
    }
}
```

Create a LowLevelMesh.Descriptor and `LowLevelMesh`, and assign your mesh data and parts:

```
func triangleMesh() throws -> LowLevelMesh {
    var desc = MyVertex.descriptor
    desc.vertexCapacity = 3
    desc.indexCapacity = 3

    let mesh = try LowLevelMesh(descriptor: desc)

    mesh.withUnsafeMutableBytes(bufferIndex: 0) { rawBytes in
        let vertices = rawBytes.bindMemory(to: MyVertex.self)
        vertices[0] = MyVertex(position: [-1, -1, 0], color: 0xFF00FF00)
        vertices[1] = MyVertex(position: [ 1, -1, 0], color: 0xFFFF0000)
        vertices[2] = MyVertex(position: [ 0,  1, 0], color: 0xFF0000FF)
    }

    mesh.withUnsafeMutableIndices { rawIndices in
        let indices = rawIndices.bindMemory(to: UInt32.self)
        indices[0] = 0
        indices[1] = 1
        indices[2] = 2
    }

    let meshBounds = BoundingBox(min: [-1, -1, 0], max: [1, 1, 0])
    mesh.parts.replaceAll([
        LowLevelMesh.Part(
            indexCount: 3,
            topology: .triangle,
            bounds: meshBounds
        )
    ])

    return mesh
}
```

To finish, create a MeshResource from the `LowLevelMesh`, and add it to a ModelComponent. You can then add this model to any Entity in your scene:

```
func triangleEntity() throws -> Entity {
    let lowLevelMesh = try triangleMesh()
    let resource = try MeshResource(from: lowLevelMesh)

    let modelComponent = ModelComponent(mesh: resource, materials: [UnlitMaterial()])

    let entity = Entity()
    entity.name = "Triangle"
    entity.components.set(modelComponent)
    entity.scale *= 0.1
    return entity
}
```

The low-level mesh creates a triangular shape in your RealityKit scene:

The MeshResource retains a reference to the `LowLevelMesh`, reflecting any changes when the renderer updates.

## Topics

### Creating a low-level mesh

init(descriptor: LowLevelMesh.Descriptor) throws

Constructs a low-level mesh from a descriptor.

### Describing a low-level mesh

let descriptor: LowLevelMesh.Descriptor

The definition of the structure of this low-level mesh.

var parts: LowLevelMesh.PartsCollection

A mutable collection of parts.

var indexCapacity: Int

The capacity of the index buffer, measured in indices.

var vertexCapacity: Int

The capacity of the vertex buffer, measured in vertices.

### Accessing mesh data on the CPU with Swift

func withUnsafeBytes(bufferIndex: Int, (UnsafeRawBufferPointer) -> Void)

Reads a Metal vertex buffer synchronously on the CPU.

func withUnsafeMutableBytes(bufferIndex: Int, (UnsafeMutableRawBufferPointer) -> Void)

Updates a Metal vertex buffer synchronously on the CPU.

func withUnsafeIndices((UnsafeRawBufferPointer) -> Void)

Reads the index buffer synchronously on the CPU.

func withUnsafeMutableIndices((UnsafeMutableRawBufferPointer) -> Void)

Updates the index buffer synchronously on the CPU.

func replaceUnsafeMutableBytes(bufferIndex: Int, (UnsafeMutableRawBufferPointer) -> Void)

Replaces a Metal vertex buffer synchronously on the CPU.

func replaceUnsafeMutableIndices((UnsafeMutableRawBufferPointer) -> Void)

Replaces the index buffer synchronously on the CPU.

### Accessing mesh data on the GPU with Metal

func read(bufferIndex: Int, using: any MTLCommandBuffer) -> any MTLBuffer

Retrieves a Metal vertex buffer at the specified index, for GPU reading.

func readIndices(using: any MTLCommandBuffer) -> any MTLBuffer

Retrieves the Metal index buffer for GPU reading.

func replace(bufferIndex: Int, using: any MTLCommandBuffer) -> any MTLBuffer

Retrieves a Metal vertex buffer you can use to replace the contents of the specified buffer on the GPU using Metal.

func replaceIndices(using: any MTLCommandBuffer) -> any MTLBuffer

Retrieves a Metal index buffer that you can use to replace the indices of this low-level mesh.

### Structures

struct Attribute

An object that determines how to store vertex attribute data in memory and map it to RealityKit shader attributes.

struct Descriptor

An object that describes the data format and layout of the buffers in a low-level mesh.

struct Layout

An object that describes a set of attributes that share a buffer index, offset, and stride.

struct Part

An object that describes a range of primitives to display, and their material index.

struct PartsCollection

An object that holds a mutable collection low-level mesh parts.

### Enumerations

enum VertexSemantic

Designates the intended usage of a vertex attribute.

## Relationships

### Conforms To

- Sendable

## See Also

### Updatable meshes

Creating a spatial drawing app with RealityKit

Use low-level mesh and texture APIs to achieve fast updates to a person’s brush strokes by integrating RealityKit with ARKit and SwiftUI.

Creating a plane with low-level mesh

Create a low-level mesh and set its vertex positions and normals to form a plane.

struct Descriptor

An object that describes the data format and layout of the buffers in a low-level mesh.

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

