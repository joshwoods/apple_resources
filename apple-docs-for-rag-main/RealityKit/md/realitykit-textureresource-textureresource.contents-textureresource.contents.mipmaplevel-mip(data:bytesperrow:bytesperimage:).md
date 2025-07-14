

- RealityKit
- TextureResource
- TextureResource.Contents
- TextureResource.Contents.MipmapLevel
-  mip(data:bytesPerRow:bytesPerImage:) 

Type Method

# mip(data:bytesPerRow:bytesPerImage:)

Specifies a multi-image mipmap level of a texture resource with pixel data that RealityKit copies from a byte buffer.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
static func mip(
    data: Data,
    bytesPerRow: Int,
    bytesPerImage: Int
) -> TextureResource.Contents.MipmapLevel
```

## Parameters 

`data`  

The source buffer.

`bytesPerRow`  

The stride in bytes between rows of texture data that RealityKit stores in the source buffer. The value needs to be a multiple of the destination texture’s pixel size, in bytes.

`bytesPerImage`  

The stride in bytes between image planes of texture data that RealityKit stores in the source buffer, needed for 3D texture mipmaps. The value needs to be a multiple of the destination texture’s pixel size, in bytes.

## See Also

### Creating a texture mipmap level

static func mip(data: Data, bytesPerRow: Int) -> TextureResource.Contents.MipmapLevel

Specifies a single mipmap level of a texture resource with pixel data that RealityKit copies from a byte buffer.

static func mip(slices: [TextureResource.Contents.Slice]) -> TextureResource.Contents.MipmapLevel

Specifies a single mipmap level of a 2D or 3D texture resource that slices provide.

static func mip(unsafeBuffer: any MTLBuffer, offset: Int, size: Int, bytesPerRow: Int) -> TextureResource.Contents.MipmapLevel

Specifies a single mipmap level of a texture resource with pixel data that RealityKit copies from a Metal buffer.

static func mip(unsafeBuffer: any MTLBuffer, offset: Int, size: Int, bytesPerRow: Int, bytesPerImage: Int) -> TextureResource.Contents.MipmapLevel

Specifies a multi-image mipmap level of a texture resource with pixel data that RealityKit copies from a Metal buffer.

