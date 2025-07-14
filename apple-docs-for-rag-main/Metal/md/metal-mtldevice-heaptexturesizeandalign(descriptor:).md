

- Metal
- MTLDevice
-  heapTextureSizeAndAlign(descriptor:) 

Instance Method

# heapTextureSizeAndAlign(descriptor:)

Returns the size and alignment, in bytes, of a texture if you create it from a heap.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
func heapTextureSizeAndAlign(descriptor desc: MTLTextureDescriptor) -> MTLSizeAndAlign
```

**Required**

## Parameters 

`desc`  

An MTLTextureDescriptor instance.

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

func heapAccelerationStructureSizeAndAlign(size: Int) -> MTLSizeAndAlign

Returns the size and alignment, in bytes, of an acceleration structure if you create it from a heap.

**Required**

func heapAccelerationStructureSizeAndAlign(descriptor: MTLAccelerationStructureDescriptor) -> MTLSizeAndAlign

Returns the size and alignment, in bytes, of an acceleration structure if you create it from a heap with a descriptor.

**Required**

struct MTLSizeAndAlign

The size and alignment of a resource, in bytes.

