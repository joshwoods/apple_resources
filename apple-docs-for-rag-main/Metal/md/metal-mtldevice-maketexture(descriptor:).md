

- Metal
- MTLDevice
-  makeTexture(descriptor:) 

Instance Method

# makeTexture(descriptor:)

Creates a new texture instance.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func makeTexture(descriptor: MTLTextureDescriptor) -> (any MTLTexture)?
```

**Required**

## Parameters 

`descriptor`  

An MTLTextureDescriptor instance.

## Return Value

A new MTLTexture instance if the method completed successfully; otherwise `nil`.

## Mentioned in 

Setting Resource Storage Modes

## See Also

### Creating Textures

func makeTexture(descriptor: MTLTextureDescriptor, iosurface: IOSurfaceRef, plane: Int) -> (any MTLTexture)?

Creates a texture instance that uses I/O surface to store its underlying data.

**Required**

func makeSharedTexture(descriptor: MTLTextureDescriptor) -> (any MTLTexture)?

Creates a texture that you can share across process boundaries.

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

