

- MetalKit
- MTKMesh
-  init(mesh:device:) 

Initializer

# init(mesh:device:)

Initializes a MetalKit mesh and its submeshes from a Model I/O mesh.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    mesh: MDLMesh,
    device: any MTLDevice
) throws
```

## Parameters 

`mesh`  

The source Model I/O mesh from which to create this MetalKit mesh.

`device`  

The Metal device on which to create MetalKit mesh resources.

## Return Value

A new MetalKit mesh object, or `nil` if an error occured.

## Discussion

This initializer does *not* initialize any children meshes of the Model I/O mesh.

All vertex buffers in the source Model I/O mesh and the index buffer of each of its submeshes must have been created with a MTKMeshBufferAllocator object.

A Model I/O submesh may have its index type and/or geometric primitive type converted to a corresponding Metal type as listed in the tables below. If the geometric primitive type cannot be converted, an error is returned through `error`.

| MDLIndexBitDepth | MTLIndexType |
|----|----|
| `MDLIndexBitDepthInvalid`  `MDLIndexBitDepthUInt8`  `MDLIndexBitDepthUInt16` | `MTLIndexTypeUInt16` |
| `MDLIndexBitDepthUInt32` | `MTLIndexTypeUInt32` |

| MDLGeometryType | MTLPrimitiveType |
|----|----|
| `MDLGeometryTypePoints` | `MTLPrimitiveTypePoint` |
| `MDLGeometryTypeLines` | `MTLPrimitiveTypeLine` |
| `MDLGeometryTypeTriangleStrips` | `MTLPrimitiveTypeTriangleStrip` |
| `MDLGeometryTypeTriangles`  `MDLGeometryTypeQuads`  `MDLGeometryTypeVariableTopology` | `MTLPrimitiveTypeTriangle` |

Note

In macOS, vertex buffers allocated from a MTKMeshBufferAllocator object are aligned to 256 bytes. Index buffers are not aligned.

