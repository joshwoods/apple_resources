

- RealityKit
- TextureResource
- TextureResource.Contents
- TextureResource.Contents.Slice
-  slice(data:bytesPerRow:) 

Type Method

# slice(data:bytesPerRow:)

Specifies a single mipmap level slice of a texture resource with pixel data that RealityKit copies from a byte buffer.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
static func slice(
    data: Data,
    bytesPerRow: Int
) -> TextureResource.Contents.Slice
```

## Parameters 

`data`  

The source buffer.

`bytesPerRow`  

The stride in bytes between rows of texture data that RealityKit stores in the source buffer. The value needs to be a multiple of the destination texture’s pixel size, in bytes.

## See Also

### Creating a texture slice

static func slice(unsafeBuffer: any MTLBuffer, offset: Int, size: Int, bytesPerRow: Int) -> TextureResource.Contents.Slice

Specifies a single mipmap level slice of a texture resource with pixel data that RealityKit copies from a Metal buffer.

