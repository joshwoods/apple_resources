

- RealityKit
- TextureResource
-  init(cubeFromEquirectangular:named:quality:faceSize:options:) 

Initializer

# init(cubeFromEquirectangular:named:quality:faceSize:options:)

Asynchronously creates a cube texture resource from an equirectangular image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
convenience init(
    cubeFromEquirectangular cgImage: CGImage,
    named resourceName: String? = nil,
    quality: TextureResource.SamplingQuality = .fast,
    faceSize: Int? = nil,
    options: TextureResource.CreateOptions
) async throws
```

## Parameters 

`cgImage`  

The source image.

`resourceName`  

A unique name for syncing the texture resource across the network. The name is empty if you don’t include one.

`quality`  

The sampling quality the initializer applies as it generates the cube texture.

`faceSize`  

The dimension of a cube face. When `faceSize` is `nil`, RealityKit computes the size based on the equirectangular image’s dimensions. RealityKit clamps the value to the source image’s height. For best results, pass values that are one-third of the cubeʻs width or less.

`options`  

A configuration for generating the texture.

## Discussion

RealityKit samples the source equirectangular image at the specified quality level to generate the cube texture.

The equirectangular image, also known as a *latitude-longitude image*, contains a flattened map of the surroundings where:

- The width is a `360°` clockwise scan along the horizon, starting from behind (+z-axis)

- The height is a -90° (bottom) to +90° (top) vertical scan

To preserve all details equirectangular images require a `2:1` aspect ratio.

Use the resulting texture to create an EnvironmentResource, or assign it to a material in Reality Composer Pro that requires a cube texture type.

```
if let source = CGImageSourceCreateWithURL(url as CFURL, nil),
    let image = CGImageSourceCreateImageAtIndex(source, 0, nil) {

    // Create a cube texture from the image.
    let cube = try await TextureResource(
        cubeFromEquirectangular: image, quality: .normal,
        options: TextureResource.CreateOptions(semantic: .hdrColor))

    // Create an environment resource from the cube texture.
    let environment = try await EnvironmentResource(
        cube: cube, options: EnvironmentResource.CreateOptions())

    await MainActor.run {
        // Assign the environment to an image-based light component.
        let lightEntity = Entity()
        lightEntity.components.set(
            ImageBasedLightComponent(source: .single(environment)))
        ...
    }
}
```

Note

EnvironmentResource.CreateOptions.SamplingQuality.high and EnvironmentResource.CreateOptions.SamplingQuality.veryHigh, along with astc(blockSize:quality:) compression options, are only available in macOS. Use these options to write optimized scenes for all target platforms when exporting from macOS with write(to:). Compression options also significantly reduce a cube’s memory and disk usage.

## See Also

### Creating a cube texture resource

convenience init(cubeFromEquirectangular: CGImage, named: String?, quality: TextureResource.SamplingQuality, faceSize: Int?, options: TextureResource.CreateOptions) throws

Synchronously creates a cube texture resource from an equirectangular image.

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

convenience init(dimensions: TextureResource.DimensionsCube, format: TextureResource.Format, contents: TextureResource.Contents) async throws

Asynchronously creates a cube texture resource from a pixel Metal buffer, or data.

struct DimensionsCube

The dimensions of the cube texture.

