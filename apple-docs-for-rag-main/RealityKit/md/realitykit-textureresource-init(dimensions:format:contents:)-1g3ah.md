

- RealityKit
- TextureResource
-  init(dimensions:format:contents:) 

Initializer

# init(dimensions:format:contents:)

Synchronously creates a 2D texture resource from a pixel Metal buffer, or data.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
convenience init(
    dimensions: TextureResource.Dimensions2D,
    format: TextureResource.Format,
    contents: TextureResource.Contents
) throws
```

## Parameters 

`dimensions`  

The width and height of the texture to create.

`format`  

The semantic interpretation of the pixel data.

`contents`  

Pixel data the system copies into the created texture.

## Discussion

Loading a TextureResource with this method blocks the main actor because it’s synchronous, so only call it from a command-line application. The method can stall a regular app, which makes it visibly hitch, and the system terminates an app if its UI becomes unresponsive. See init(named:in:) for an example that demonstrates how to safely load content.

RealityKit efficiently creates a 2D texture from raw pixel bytes, with full control over the values and pixel format. See init(dimensions:format:contents:) for more details.

## See Also

### Creating a 2D texture resource

convenience init(image: CGImage, withName: String?, options: TextureResource.CreateOptions) async throws

Asynchronously creates a texture resource from an in-memory Core Graphics image.

convenience init(image: CGImage, withName: String?, options: TextureResource.CreateOptions) throws

Synchronously creates a texture resource from an in-memory Core Graphics image.

convenience init(dimensions: TextureResource.Dimensions2D, format: TextureResource.Format, contents: TextureResource.Contents) async throws

Asynchronously creates a 2D texture resource from a pixel Metal buffer, or data.

struct Dimensions2D

The dimensions of a 2D texture.

