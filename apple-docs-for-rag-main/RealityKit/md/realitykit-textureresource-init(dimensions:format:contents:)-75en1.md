

- RealityKit
- TextureResource
-  init(dimensions:format:contents:) 

Initializer

# init(dimensions:format:contents:)

Asynchronously creates a cube texture resource from a pixel Metal buffer, or data.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
convenience init(
    dimensions: TextureResource.DimensionsCube,
    format: TextureResource.Format,
    contents: TextureResource.Contents
) async throws
```

## Parameters 

`dimensions`  

The dimensions of the cube texture to create.

`format`  

The semantic interpretation of the pixel data.

`contents`  

Pixel data the system copies into the created texture.

## Discussion

RealityKit efficiently creates a cube texture from raw pixel bytes, with full control over the values and pixel format. Use the resulting texture to create an EnvironmentResource, or assign it to a material in Reality Composer Pro that requires a cube texture type.

```
var mips: [TextureResource.Contents.MipmapLevel] = []

// Create the various mipmap levels.
// A `bufferMipsInfo` structure describes the mipmap packing in the source `MTLBuffer`.
for mipInfo in bufferMipsInfo {
    var faceSlices = [TextureResource.Contents.Slice]()
    for faceInfo in mipInfo {
        faceSlices.append(.slice(
            unsafeBuffer: buffer,
            offset: faceInfo.offset,
            size: faceInfo.size,
            bytesPerRow: faceInfo.width * bytesPerPixel
        ))
    }
    mips.append(.mip(slices: faceSlices))
}

let texture = try TextureResource(
    dimensions: .dimensions(faceSize: faceSize),
    format: .color(.displayP3, pixelFormat: .rgba8Unorm),
    contents: TextureResource.Contents(mipmapLevels: mips)
)
```

See init(named:in:) for an example of optimally loading textures with other content.

## See Also

### Creating a cube texture resource

convenience init(cubeFromEquirectangular: CGImage, named: String?, quality: TextureResource.SamplingQuality, faceSize: Int?, options: TextureResource.CreateOptions) throws

Synchronously creates a cube texture resource from an equirectangular image.

convenience init(cubeFromEquirectangular: CGImage, named: String?, quality: TextureResource.SamplingQuality, faceSize: Int?, options: TextureResource.CreateOptions) async throws

Asynchronously creates a cube texture resource from an equirectangular image.

convenience init(cubeFromImage: CGImage, named: String?, options: TextureResource.CreateOptions) throws

Synchronously creates a cube texture resource from a 2D image of cube faces.

convenience init(cubeFromImage: CGImage, named: String?, options: TextureResource.CreateOptions) async throws

Asynchronously creates a cube texture resource from a 2D image of cube faces.

static func cube(slices: [CGImage], named: String?, options: TextureResource.CreateOptions) async throws -> TextureResource

Asynchronously creates a cube texture resource from face images.

static func cube(slices: [CGImage], named: String?, options: TextureResource.CreateOptions) throws -> TextureResource

Synchronously creates a cube texture resource from face images.

convenience init(dimensions: TextureResource.DimensionsCube, format: TextureResource.Format, contents: TextureResource.Contents) throws

Synchronously creates a cube texture resource from a pixel Metal buffer, or data.

struct DimensionsCube

The dimensions of the cube texture.

