

- Metal
- MTLRenderPipelineDescriptor
-  vertexDescriptor 

Instance Property

# vertexDescriptor

The organization of vertex data in an attribute’s argument table.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
@NSCopying
var vertexDescriptor: MTLVertexDescriptor? { get set }
```

## Discussion

A MTLVertexDescriptor object is used to describe the organization of per-vertex input structs passed in an argument of a vertex shader function.

