

- MetalKit
- MTKMeshBuffer
-  allocator 

Instance Property

# allocator

The allocator object used to create this mesh buffer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var allocator: MTKMeshBufferAllocator { get }
```

## Discussion

The allocator uses Model I/O for copy and re-layout operations, such as when a new vertex descriptor is applied to an existing vertex buffer.

## See Also

### Originating Objects

var type: MDLMeshBufferType

The type of data contained in the originating Model I/O buffer.

