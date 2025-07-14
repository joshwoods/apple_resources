

- Metal
- MTLHeap
-  makeBuffer(length:options:offset:) 

Instance Method

# makeBuffer(length:options:offset:)

Creates a buffer at a specified offset on the heap.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func makeBuffer(
    length: Int,
    options: MTLResourceOptions = [],
    offset: Int
) -> (any MTLBuffer)?
```

**Required**

## Parameters 

`length`  

The size of the buffer, in bytes.

`options`  

Options that describe the properties of the buffer. The buffer’s storage mode and CPU cache mode must match the heap’s storageMode and cpuCacheMode values.

`offset`  

The distance, in bytes, to place the buffer relative to the start of the heap.

## Return Value

A new buffer, or `nil` if the heap is not a placement heap.

## Discussion

The heap’s type must be MTLHeapType.placement.

Use the heapBufferSizeAndAlign(length:options:) method to determine the required size and alignment. If you don’t align the buffer correctly or it extends past the end of the heap, the behavior is undefined.

Any resources in the heap within an overlapping half-open range `[offset, offset + requiredSize)` are implicitly aliased with the new resource.

## See Also

### Creating Resources on the Heap

func makeBuffer(length: Int, options: MTLResourceOptions) -> (any MTLBuffer)?

Creates a buffer on the heap.

**Required**

func makeTexture(descriptor: MTLTextureDescriptor) -> (any MTLTexture)?

Creates a texture on the heap.

**Required**

func makeTexture(descriptor: MTLTextureDescriptor, offset: Int) -> (any MTLTexture)?

Creates a texture at a specified offset on the heap.

**Required**

