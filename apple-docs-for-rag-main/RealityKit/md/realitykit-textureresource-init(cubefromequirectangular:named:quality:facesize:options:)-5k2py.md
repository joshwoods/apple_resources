

- RealityKit
- TextureResource
-  init(cubeFromEquirectangular:named:quality:faceSize:options:) 

Initializer

# init(cubeFromEquirectangular:named:quality:faceSize:options:)

Synchronously creates a cube texture resource from an equirectangular image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
convenience init(
    cubeFromEquirectangular cgImage: CGImage,
    named resourceName: String? = nil,
    quality: TextureResource.SamplingQuality = .fast,
    faceSize: Int? = nil,
    options: TextureResource.CreateOptions
) throws
```

## Parameters 

`cgImage`  

The source image.

`resourceName`  

A unique name for syncing the texture resource across the network. The name is empty if you don’t include one.

`quality`  

The sampling quality the initializer applies as it generates the cube texture.

`faceSize`  

The length of the cube’s sides, in pixels. When `faceSize` is `nil`, RealityKit computes the size based on the equirectangular image’s dimensions. RealityKit clamps the value to the source image’s height. For best results, pass values that are one-third of the cubeʻs width or less.

`options`  

A configuration for generating the texture.

## Discussion

Loading a TextureResource with this method blocks the main actor because it’s synchronous, so only call it from a command-line application. The method can stall a regular app, which makes it visibly hitch, and the system terminates an app if its UI becomes unresponsive. See init(named:in:) for an example that demonstrates how to safely load content.

RealityKit samples the source equirectangular image at the specified quality level to generate the cube texture. See init(cubeFromEquirectangular:named:quality:faceSize:options:) for equirectangular image requirements.

```
if let source = CGImageSourceCreateWithURL(url as CFURL, nil),
    let image = CGImageSourceCreateImageAtIndex(source, 0, nil) {

    // Create a cube texture from the image.
    let cube = try TextureResource(
        cubeFromEquirectangular: image, quality: .normal,
        options: TextureResource.CreateOptions(semantic: .hdrColor))

    // Create an environment resource from the cube texture.
    let environment = try EnvironmentResource(
        cube: cube, options: EnvironmentResource.CreateOptions())

    // Assign the environment to an image-based light component.
    let lightEntity = Entity()
    lightEntity.components.set(ImageBasedLightComponent(
        source: .single(environment)))
    ...
}
```

## See Also

### Creating a cube texture resource

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

convenience init(dimensions: TextureResource.DimensionsCube, format: TextureResource.Format, contents: TextureResource.Contents) async throws

Asynchronously creates a cube texture resource from a pixel Metal buffer, or data.

struct DimensionsCube

The dimensions of the cube texture.

