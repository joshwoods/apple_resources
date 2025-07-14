

- RealityKit
- TextureResource
-  cube(slices:named:options:) 

Type Method

# cube(slices:named:options:)

Asynchronously creates a cube texture resource from face images.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
static func cube(
    slices: [CGImage],
    named resourceName: String? = nil,
    options: TextureResource.CreateOptions
) async throws -> TextureResource
```

## Parameters 

`slices`  

The source images for each cube face in \[`+X`, `-X`, `+Y`, `-Y`, `+Z`, `-Z`\] order. All images need to be square, and of equal size.

`resourceName`  

A unique name for syncing the texture resource across the network. The name is empty if you don’t include one.

`options`  

A configuration for generating the texture.

## Discussion

Provide the cube faces in the following order: \[`+X`, `-X`, `+Y`, `-Y`, `+Z`, `-Z`\].

|  |  |  |  |  |  |
|----|----|----|----|----|----|

Use the resulting texture to create an EnvironmentResource, or assign it to a material in Reality Composer Pro that requires a cube texture type.

```
// Create a cube texture from image slices.
let cube = try await TextureResource.cube(
    slices: [posXImage, negXImage, posYImage, negYImage, posZImage, negZImage],
    options: TextureResource.CreateOptions(semantic: .hdrColor)
)

// Create an environment resource from the cube texture.
let environment = try await EnvironmentResource(
    cube: cube,
    options: EnvironmentResource.CreateOptions()
)

await MainActor.run {
    // Assign the environment to an image-based light component.
    let lightEntity = Entity()
    lightEntity.components.set(ImageBasedLightComponent(
        source: .single(environment)))
    ...
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

convenience init(cubeFromImage: CGImage, named: String?, options: TextureResource.CreateOptions) async throws

Asynchronously creates a cube texture resource from a 2D image of cube faces.

static func cube(slices: [CGImage], named: String?, options: TextureResource.CreateOptions) throws -> TextureResource

Synchronously creates a cube texture resource from face images.

convenience init(dimensions: TextureResource.DimensionsCube, format: TextureResource.Format, contents: TextureResource.Contents) throws

Synchronously creates a cube texture resource from a pixel Metal buffer, or data.

convenience init(dimensions: TextureResource.DimensionsCube, format: TextureResource.Format, contents: TextureResource.Contents) async throws

Asynchronously creates a cube texture resource from a pixel Metal buffer, or data.

struct DimensionsCube

The dimensions of the cube texture.

