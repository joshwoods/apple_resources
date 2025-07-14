

- RealityKit
- TextureResource
-  init(dimensions:format:contents:) 

Initializer

# init(dimensions:format:contents:)

Asynchronously creates a 2D array texture resource from a pixel Metal buffer, or data.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
convenience init(
    dimensions: TextureResource.Dimensions2DArray,
    format: TextureResource.Format,
    contents: TextureResource.Contents
) async throws
```

## Parameters 

`dimensions`  

The dimensions of the 2D array texture to create.

`format`  

The semantic interpretation of the pixel data.

`contents`  

Pixel data the system copies into the created texture.

## Discussion

RealityKit efficiently creates a 2D array texture from raw pixel bytes, with full control over the values and pixel format. You can assign the resulting texture to a material you create in Reality Composer Pro that requires a 2D texture array.

```
var mips: [TextureResource.Contents.MipmapLevel] = []

// Create the various mipmap levels.
// A `bufferMipsInfo` structure describes the mipmap packing in the source `MTLBuffer`.
for mipInfo in bufferMipsInfo {
    var slices = [TextureResource.Contents.Slice]()
    for sliceInfo in mipInfo {
        slices.append(.slice(
            unsafeBuffer: buffer,
            offset: sliceInfo.offset,
            size: sliceInfo.size,
            bytesPerRow: sliceInfo.width * bytesPerPixel
        ))
    }
    mips.append(.mip(slices: slices))
}

let texture = try TextureResource(
    dimensions: .dimensions(width: width, height: height, length: arrayLength),
    format: .color(.displayP3, pixelFormat: .rgba8Unorm),
    contents: TextureResource.Contents(mipmapLevels: mips)
)
```

See init(named:in:) for an example of optimally loading textures with other content.

## See Also

### Creating a 2D array texture resource

static func texture2DArray(slices: [CGImage], named: String?, options: TextureResource.CreateOptions) async throws -> TextureResource

Asynchronously creates a 2D texture array by generating it from images.

static func texture2DArray(slices: [CGImage], named: String?, options: TextureResource.CreateOptions) throws -> TextureResource

Synchronously creates a 2D texture array by generating it from images.

convenience init(dimensions: TextureResource.Dimensions2DArray, format: TextureResource.Format, contents: TextureResource.Contents) throws

Synchronously creates a 2D array texture resource from a pixel Metal buffer, or data.

struct Dimensions2DArray

The dimensions of the 2D array texture.

