

- Metal
- MTLDevice
-  makeSharedTexture(descriptor:) 

Instance Method

# makeSharedTexture(descriptor:)

Creates a texture that you can share across process boundaries.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.14+tvOS 13.0+visionOS 1.0+

``` source
func makeSharedTexture(descriptor: MTLTextureDescriptor) -> (any MTLTexture)?
```

**Required**

## Parameters 

`descriptor`  

An MTLTextureDescriptor instance.

## Return Value

A new MTLTexture instance if the method completed successfully; otherwise `nil`.

## Discussion

You can create a shared texture but only with storageModePrivate. You can share the texture with another process by:

1.  Creating a texture handle (see makeSharedTextureHandle())

2.  Passing the texture handle to the other process

3.  Creating a texture in the other process by calling the makeSharedTexture(handle:)method

Important

You can share a texture with another process that uses the same GPU, but not with a different GPU.

## See Also

### Creating Textures

func makeTexture(descriptor: MTLTextureDescriptor) -> (any MTLTexture)?

Creates a new texture instance.

**Required**

func makeTexture(descriptor: MTLTextureDescriptor, iosurface: IOSurfaceRef, plane: Int) -> (any MTLTexture)?

Creates a texture instance that uses I/O surface to store its underlying data.

**Required**

func makeSharedTexture(handle: MTLSharedTextureHandle) -> (any MTLTexture)?

Creates a texture that references a shared texture.

**Required**

func minimumLinearTextureAlignment(for: MTLPixelFormat) -> Int

Returns the minimum alignment the GPU device requires to create a linear texture from a buffer.

**Required**

func minimumTextureBufferAlignment(for: MTLPixelFormat) -> Int

Returns the minimum alignment the GPU device requires to create a texture buffer from a buffer.

**Required**

