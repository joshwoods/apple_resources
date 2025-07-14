

- Metal
- MTLHeap
-  makeTexture(descriptor:offset:) 

Instance Method

# makeTexture(descriptor:offset:)

Creates a texture at a specified offset on the heap.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func makeTexture(
    descriptor: MTLTextureDescriptor,
    offset: Int
) -> (any MTLTexture)?
```

**Required**

## Parameters 

`descriptor`  

A descriptor object that describes the properties of the texture.

`offset`  

The distance, in bytes, to place the texture relative to the start of the heap.

## Return Value

A new texture, or `nil` if the heap is not a placement heap.

## Discussion

The heap’s type must be MTLHeapType.placement.

The texture’s CPU cache mode must match the heap’s cpuCacheMode value. The texture’s storage mode must either match the heap’s storageMode value or be a MTLStorageMode.memoryless value.

Use the heapBufferSizeAndAlign(length:options:) to determine the required size and alignment. If you don’t align the texture correctly or it extends past the end of the heap, the behavior is undefined.

Any resources in the heap within an overlapping half-open range `[offset, offset + requiredSize)` are implicitly aliased with the new resource.

## See Also

### Creating Resources on the Heap

func makeBuffer(length: Int, options: MTLResourceOptions) -> (any MTLBuffer)?

Creates a buffer on the heap.

**Required**

func makeTexture(descriptor: MTLTextureDescriptor) -> (any MTLTexture)?

Creates a texture on the heap.

**Required**

func makeBuffer(length: Int, options: MTLResourceOptions, offset: Int) -> (any MTLBuffer)?

Creates a buffer at a specified offset on the heap.

**Required**

