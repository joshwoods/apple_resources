

- Metal
- MTLDevice
-  minimumLinearTextureAlignment(for:) 

Instance Method

# minimumLinearTextureAlignment(for:)

Returns the minimum alignment the GPU device requires to create a linear texture from a buffer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func minimumLinearTextureAlignment(for format: MTLPixelFormat) -> Int
```

**Required**

## Parameters 

`format`  

An MTLPixelFormat instance that can’t be any of the depth, stencil, or compressed pixel formats.

## Mentioned in 

Developing Metal apps that run in Simulator

## Discussion

Metal aligns linear textures to their minimum alignment value, which directly affects the makeTexture(descriptor:offset:bytesPerRow:) method’s `offset` and `bytesPerRow` parameters.

## See Also

### Creating Textures

func makeTexture(descriptor: MTLTextureDescriptor) -> (any MTLTexture)?

Creates a new texture instance.

**Required**

func makeTexture(descriptor: MTLTextureDescriptor, iosurface: IOSurfaceRef, plane: Int) -> (any MTLTexture)?

Creates a texture instance that uses I/O surface to store its underlying data.

**Required**

func makeSharedTexture(descriptor: MTLTextureDescriptor) -> (any MTLTexture)?

Creates a texture that you can share across process boundaries.

**Required**

func makeSharedTexture(handle: MTLSharedTextureHandle) -> (any MTLTexture)?

Creates a texture that references a shared texture.

**Required**

func minimumTextureBufferAlignment(for: MTLPixelFormat) -> Int

Returns the minimum alignment the GPU device requires to create a texture buffer from a buffer.

**Required**

