

- Metal
- MTLDevice
-  makeHeap(descriptor:) 

Instance Method

# makeHeap(descriptor:)

Creates a new GPU heap instance.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
func makeHeap(descriptor: MTLHeapDescriptor) -> (any MTLHeap)?
```

**Required**

## Parameters 

`descriptor`  

An MTLHeapDescriptor instance.

## Return Value

A new MTLHeap instance if the method completed successfully; otherwise nil.

## Discussion

For more information about using heaps, see Memory Heaps.

## See Also

### Working with Resource Heaps

func heapBufferSizeAndAlign(length: Int, options: MTLResourceOptions) -> MTLSizeAndAlign

Returns the size and alignment, in bytes, of a buffer if you create it from a heap.

**Required**

func heapTextureSizeAndAlign(descriptor: MTLTextureDescriptor) -> MTLSizeAndAlign

Returns the size and alignment, in bytes, of a texture if you create it from a heap.

**Required**

func heapAccelerationStructureSizeAndAlign(size: Int) -> MTLSizeAndAlign

Returns the size and alignment, in bytes, of an acceleration structure if you create it from a heap.

**Required**

func heapAccelerationStructureSizeAndAlign(descriptor: MTLAccelerationStructureDescriptor) -> MTLSizeAndAlign

Returns the size and alignment, in bytes, of an acceleration structure if you create it from a heap with a descriptor.

**Required**

struct MTLSizeAndAlign

The size and alignment of a resource, in bytes.

