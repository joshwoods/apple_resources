

- RealityKit
- TextureResource
-  init(cubeFromImage:named:options:) 

Initializer

# init(cubeFromImage:named:options:)

Asynchronously creates a cube texture resource from a 2D image of cube faces.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
convenience init(
    cubeFromImage cgImage: CGImage,
    named resourceName: String? = nil,
    options: TextureResource.CreateOptions
) async throws
```

## Parameters 

`cgImage`  

The source image.

`resourceName`  

A unique name for syncing the texture resource across the network. The name is empty if you don’t include one.

`options`  

A configuration for generating the texture.

## Discussion

RealityKit extracts the cube faces from the source 2D image using a convention based on its aspect ratio, which needs to be one of the following:

- If `height == 6 * width`, RealityKit treats the source image as a vertical strip of the cube faces, containing \[+X, -X, +Y, -Y, +Z, -Z\] from top to bottom:

- If `6 * height == width`, RealityKit treats the source image as a horizontal strip of the cube faces, containing \[+X, -X, +Y, -Y, +Z, -Z\] from left to right:

- If `height / 3 == width / 4`, RealityKit treats the source image as a cross layout of the cube faces as follows:

```
    [+Y]
[+X][-Z][-X][+Z]
    [-Y]
```

Use the resulting texture to create an EnvironmentResource, or assign it to a material in Reality Composer Pro that requires a cube texture type.

```
if let source = CGImageSourceCreateWithURL(url as CFURL, nil),
    let image = CGImageSourceCreateImageAtIndex(source, 0, nil) {

    // Create a cube texture from the image.
    let cube = try await TextureResource(
        cubeFromImage: image, options: TextureResource.CreateOptions(semantic: .hdrColor))

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

## See Also

### Creating a cube texture resource

convenience init(cubeFromEquirectangular: CGImage, named: String?, quality: TextureResource.SamplingQuality, faceSize: Int?, options: TextureResource.CreateOptions) throws

Synchronously creates a cube texture resource from an equirectangular image.

convenience init(cubeFromEquirectangular: CGImage, named: String?, quality: TextureResource.SamplingQuality, faceSize: Int?, options: TextureResource.CreateOptions) async throws

Asynchronously creates a cube texture resource from an equirectangular image.

convenience init(cubeFromImage: CGImage, named: String?, options: TextureResource.CreateOptions) throws

Synchronously creates a cube texture resource from a 2D image of cube faces.

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

