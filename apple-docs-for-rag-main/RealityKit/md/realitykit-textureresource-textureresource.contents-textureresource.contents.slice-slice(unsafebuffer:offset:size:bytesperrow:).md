

- RealityKit
- TextureResource
- TextureResource.Contents
- TextureResource.Contents.Slice
-  slice(unsafeBuffer:offset:size:bytesPerRow:) 

Type Method

# slice(unsafeBuffer:offset:size:bytesPerRow:)

Specifies a single mipmap level slice of a texture resource with pixel data that RealityKit copies from a Metal buffer.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
static func slice(
    unsafeBuffer buffer: any MTLBuffer,
    offset: Int = 0,
    size: Int,
    bytesPerRow: Int
) -> TextureResource.Contents.Slice
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

## Discussion

Important

A TextureResource.Contents.Slice that you create with this function and use to create a TextureResource copies from the source buffer. That copy occurs when initializing the texture resource. The caller is responsible for ensuring that the system doesn’t modify the source Metal buffer while copying it to a texture.

## See Also

### Creating a texture slice

static func slice(data: Data, bytesPerRow: Int) -> TextureResource.Contents.Slice

Specifies a single mipmap level slice of a texture resource with pixel data that RealityKit copies from a byte buffer.

