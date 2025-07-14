

- Metal
- MTLHeap
-  makeBuffer(length:options:) 

Instance Method

# makeBuffer(length:options:)

Creates a buffer on the heap.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
func makeBuffer(
    length: Int,
    options: MTLResourceOptions = []
) -> (any MTLBuffer)?
```

**Required**

## Parameters 

`length`  

The size, in bytes, of the buffer.

`options`  

Options that describe the properties of the buffer.

## Return Value

A new buffer object backed by heap memory, or `nil` if the heap memory is full.

## Discussion

The heap’s type must be MTLHeapType.automatic.

The buffer’s storage mode and CPU cache mode must match the heap’s storageMode and cpuCacheMode values.

## See Also

### Creating Resources on the Heap

func makeTexture(descriptor: MTLTextureDescriptor) -> (any MTLTexture)?

Creates a texture on the heap.

**Required**

func makeBuffer(length: Int, options: MTLResourceOptions, offset: Int) -> (any MTLBuffer)?

Creates a buffer at a specified offset on the heap.

**Required**

func makeTexture(descriptor: MTLTextureDescriptor, offset: Int) -> (any MTLTexture)?

Creates a texture at a specified offset on the heap.

**Required**

