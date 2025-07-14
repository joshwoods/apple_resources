

- Metal
- MTLDevice
-  minimumTextureBufferAlignment(for:) 

Instance Method

# minimumTextureBufferAlignment(for:)

Returns the minimum alignment the GPU device requires to create a texture buffer from a buffer.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
func minimumTextureBufferAlignment(for format: MTLPixelFormat) -> Int
```

**Required**

## Parameters 

`format`  

An MTLPixelFormat instance.

## Discussion

Metal aligns textures to their minimum alignment value, which directly affects the makeTexture(descriptor:offset:bytesPerRow:) method’s `offset` and `bytesPerRow` parameters.

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

func minimumLinearTextureAlignment(for: MTLPixelFormat) -> Int

Returns the minimum alignment the GPU device requires to create a linear texture from a buffer.

**Required**

