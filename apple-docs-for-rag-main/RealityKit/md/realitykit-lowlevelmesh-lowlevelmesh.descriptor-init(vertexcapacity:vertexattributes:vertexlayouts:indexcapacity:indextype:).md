

- RealityKit
- LowLevelMesh
- LowLevelMesh.Descriptor
-  init(vertexCapacity:vertexAttributes:vertexLayouts:indexCapacity:indexType:) 

Initializer

# init(vertexCapacity:vertexAttributes:vertexLayouts:indexCapacity:indexType:)

Creates a descriptor for a low-level mesh.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    vertexCapacity: Int = 0,
    vertexAttributes: [LowLevelMesh.Attribute] = [Attribute](),
    vertexLayouts: [LowLevelMesh.Layout] = [Layout](),
    indexCapacity: Int = 0,
    indexType: MTLIndexType = MTLIndexType.uint32
)
```

## Parameters 

`vertexCapacity`  

The maximum number of vertices the system can store in the mesh.

`vertexAttributes`  

The attributes of the vertices.

`vertexLayouts`  

The layouts for the vertex buffers.

`indexCapacity`  

The maximum number of vertices the system can store in a single buffer.

`indexType`  

The index type to use for the mesh.

## Discussion

To create a new LowLevelMesh, first create a `Descriptor` object and set its property values, then use that `Descriptor` with init(descriptor:).

