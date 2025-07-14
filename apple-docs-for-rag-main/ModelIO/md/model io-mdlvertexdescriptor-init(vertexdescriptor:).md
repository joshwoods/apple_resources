

- Model I/O
- MDLVertexDescriptor
-  init(vertexDescriptor:) 

Initializer

# init(vertexDescriptor:)

Creates a new vertex descriptor by performing a deep copy of the specified vertex descriptor.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(vertexDescriptor: MDLVertexDescriptor)
```

## Parameters 

`vertexDescriptor`  

The vertex descriptor from which to copy information.

## Return Value

A new vertex descriptor that is an indpendent copy of the specified vertex descriptor.

## Discussion

A vertex descriptor does not own vertex data—vertex data belongs to the vertexBuffers property of the mesh that owns a vertex descriptor—so this method does not copy vertex data. A call to the copy() or copy(with:) method uses this initializer to produce a fully independent copy of the original instance.

