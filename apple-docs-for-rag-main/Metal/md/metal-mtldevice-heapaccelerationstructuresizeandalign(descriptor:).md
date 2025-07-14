

- Metal
- MTLDevice
-  heapAccelerationStructureSizeAndAlign(descriptor:) 

Instance Method

# heapAccelerationStructureSizeAndAlign(descriptor:)

Returns the size and alignment, in bytes, of an acceleration structure if you create it from a heap with a descriptor.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func heapAccelerationStructureSizeAndAlign(descriptor: MTLAccelerationStructureDescriptor) -> MTLSizeAndAlign
```

**Required**

## Parameters 

`descriptor`  

An MTLAccelerationStructureDescriptor instance.

## Return Value

An MTLSizeAndAlign instance.

## Discussion

Use this method to help estimate an appropriate size for a new heap before you create it.

## See Also

### Working with Resource Heaps

func makeHeap(descriptor: MTLHeapDescriptor) -> (any MTLHeap)?

Creates a new GPU heap instance.

**Required**

func heapBufferSizeAndAlign(length: Int, options: MTLResourceOptions) -> MTLSizeAndAlign

Returns the size and alignment, in bytes, of a buffer if you create it from a heap.

**Required**

func heapTextureSizeAndAlign(descriptor: MTLTextureDescriptor) -> MTLSizeAndAlign

Returns the size and alignment, in bytes, of a texture if you create it from a heap.

**Required**

func heapAccelerationStructureSizeAndAlign(size: Int) -> MTLSizeAndAlign

Returns the size and alignment, in bytes, of an acceleration structure if you create it from a heap.

**Required**

struct MTLSizeAndAlign

The size and alignment of a resource, in bytes.

