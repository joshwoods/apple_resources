

- Metal
- MTLDevice
-  makeTexture(descriptor:iosurface:plane:) 

Instance Method

# makeTexture(descriptor:iosurface:plane:)

Creates a texture instance that uses I/O surface to store its underlying data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.11+tvOS 11.0+visionOS 1.0+

``` source
func makeTexture(
    descriptor: MTLTextureDescriptor,
    iosurface: IOSurfaceRef,
    plane: Int
) -> (any MTLTexture)?
```

**Required**

## Parameters 

`descriptor`  

An MTLTextureDescriptor instance.

`iosurface`  

An `IOSurfaceRef` instance.

`plane`  

A plane within i`osurface` the method sets as the texture’s underlying data.

## Return Value

A new MTLTexture instance if the method completed successfully; otherwise `nil`.

## See Also

### Creating Textures

func makeTexture(descriptor: MTLTextureDescriptor) -> (any MTLTexture)?

Creates a new texture instance.

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

