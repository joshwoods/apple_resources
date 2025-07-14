

- RealityKit
- TextureResource
-  init(image:withName:options:) 

Initializer

# init(image:withName:options:)

Asynchronously creates a texture resource from an in-memory Core Graphics image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
convenience init(
    image cgImage: CGImage,
    withName resourceName: String? = nil,
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

This method creates a texture resource from an existing CGImage with specific options.

RealityKit uses the resource name to identify resources, and to match texture resources between networked peers. Specify a unique name for each texture resource you load or generate.

## See Also

### Creating a 2D texture resource

convenience init(image: CGImage, withName: String?, options: TextureResource.CreateOptions) throws

Synchronously creates a texture resource from an in-memory Core Graphics image.

convenience init(dimensions: TextureResource.Dimensions2D, format: TextureResource.Format, contents: TextureResource.Contents) throws

Synchronously creates a 2D texture resource from a pixel Metal buffer, or data.

convenience init(dimensions: TextureResource.Dimensions2D, format: TextureResource.Format, contents: TextureResource.Contents) async throws

Asynchronously creates a 2D texture resource from a pixel Metal buffer, or data.

struct Dimensions2D

The dimensions of a 2D texture.

