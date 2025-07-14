

- Metal
- MTLHeap
-  makeTexture(descriptor:) 

Instance Method

# makeTexture(descriptor:)

Creates a texture on the heap.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
func makeTexture(descriptor: MTLTextureDescriptor) -> (any MTLTexture)?
```

**Required**

## Parameters 

`descriptor`  

A descriptor object that describes the properties of the texture.

## Return Value

A new texture object backed by heap memory, or `nil` if the heap memory is full.

## Discussion

The heap’s type must be MTLHeapType.automatic.

The texture’s CPU cache mode must match the heap’s cpuCacheMode value. The texture’s storage mode must either match the heap’s storageMode value or be a MTLStorageMode.memoryless value.

## See Also

### Creating Resources on the Heap

func makeBuffer(length: Int, options: MTLResourceOptions) -> (any MTLBuffer)?

Creates a buffer on the heap.

**Required**

func makeBuffer(length: Int, options: MTLResourceOptions, offset: Int) -> (any MTLBuffer)?

Creates a buffer at a specified offset on the heap.

**Required**

func makeTexture(descriptor: MTLTextureDescriptor, offset: Int) -> (any MTLTexture)?

Creates a texture at a specified offset on the heap.

**Required**

