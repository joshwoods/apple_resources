

- Metal
- MTLDevice
-  makeSharedTexture(handle:) 

Instance Method

# makeSharedTexture(handle:)

Creates a texture that references a shared texture.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.14+tvOS 13.0+visionOS 1.0+

``` source
func makeSharedTexture(handle sharedHandle: MTLSharedTextureHandle) -> (any MTLTexture)?
```

**Required**

## Parameters 

`sharedHandle`  

An MTLSharedTextureHandle instance, typically from another process using the same GPU device.

## Return Value

A new MTLTexture instance if the method completed successfully; otherwise `nil`.

## Discussion

Call this method from the same MTLDevice instance that created the shared texture instance.

Tip

You can identify the correct device with the texture handle’s device property.

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

func minimumLinearTextureAlignment(for: MTLPixelFormat) -> Int

Returns the minimum alignment the GPU device requires to create a linear texture from a buffer.

**Required**

func minimumTextureBufferAlignment(for: MTLPixelFormat) -> Int

Returns the minimum alignment the GPU device requires to create a texture buffer from a buffer.

**Required**

