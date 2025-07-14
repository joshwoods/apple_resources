

- RealityKit
- TextureResource
- TextureResource.Contents
- TextureResource.Contents.MipmapLevel
-  mip(unsafeBuffer:offset:size:bytesPerRow:bytesPerImage:) 

Type Method

# mip(unsafeBuffer:offset:size:bytesPerRow:bytesPerImage:)

Specifies a multi-image mipmap level of a texture resource with pixel data that RealityKit copies from a Metal buffer.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
static func mip(
    unsafeBuffer buffer: any MTLBuffer,
    offset: Int = 0,
    size: Int,
    bytesPerRow: Int,
    bytesPerImage: Int
) -> TextureResource.Contents.MipmapLevel
```

## Parameters 

`buffer`  

The source buffer. Don’t modify this buffer while using it as the source of a copy operation.

`offset`  

The byte position in the source buffer where the copying starts. The offset needs to be a multiple of the destination texture’s pixel size, in bytes.

`size`  

The number of bytes in the source buffer (starting from `offset`) available for copying.

`bytesPerRow`  

The stride in bytes between rows of texture data that RealityKit stores in the source buffer. The value needs to be a multiple of the destination texture’s pixel size, in bytes.

`bytesPerImage`  

The stride in bytes between image planes of texture data that RealityKit stores in the source buffer, needed for 3D texture mipmaps. The value needs to be a multiple of the destination texture’s pixel size, in bytes.

## Discussion

Important

A TextureResource.Contents.MipmapLevel that you create with this function and use to create a TextureResource copies from the source buffer. That copy occurs when initializing the texture resource. The caller is responsible for ensuring that the system doesn’t modify the source Metal buffer while copying it to a texture.

## See Also

### Creating a texture mipmap level

static func mip(data: Data, bytesPerRow: Int) -> TextureResource.Contents.MipmapLevel

Specifies a single mipmap level of a texture resource with pixel data that RealityKit copies from a byte buffer.

static func mip(data: Data, bytesPerRow: Int, bytesPerImage: Int) -> TextureResource.Contents.MipmapLevel

Specifies a multi-image mipmap level of a texture resource with pixel data that RealityKit copies from a byte buffer.

static func mip(slices: [TextureResource.Contents.Slice]) -> TextureResource.Contents.MipmapLevel

Specifies a single mipmap level of a 2D or 3D texture resource that slices provide.

static func mip(unsafeBuffer: any MTLBuffer, offset: Int, size: Int, bytesPerRow: Int) -> TextureResource.Contents.MipmapLevel

Specifies a single mipmap level of a texture resource with pixel data that RealityKit copies from a Metal buffer.

