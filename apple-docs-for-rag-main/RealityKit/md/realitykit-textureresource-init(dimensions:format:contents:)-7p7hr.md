

- RealityKit
- TextureResource
-  init(dimensions:format:contents:) 

Initializer

# init(dimensions:format:contents:)

Synchronously creates a 2D array texture resource from a pixel Metal buffer, or data.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
convenience init(
    dimensions: TextureResource.Dimensions2DArray,
    format: TextureResource.Format,
    contents: TextureResource.Contents
) throws
```

## Parameters 

`dimensions`  

The dimensions of the 2D array texture to create.

`format`  

The semantic interpretation of the pixel data.

`contents`  

Pixel data the system copies into the created texture.

## Discussion

Loading a TextureResource with this method blocks the main actor because it’s synchronous, so only call it from a command-line application. The method can stall a regular app, which makes it visibly hitch, and the system terminates an app if its UI becomes unresponsive. See init(named:in:) for an example that demonstrates how to safely load content.

RealityKit efficiently creates a 2D array texture from raw pixel bytes, with full control over the values and pixel format. See init(dimensions:format:contents:) for more details.

## See Also

### Creating a 2D array texture resource

static func texture2DArray(slices: [CGImage], named: String?, options: TextureResource.CreateOptions) async throws -> TextureResource

Asynchronously creates a 2D texture array by generating it from images.

static func texture2DArray(slices: [CGImage], named: String?, options: TextureResource.CreateOptions) throws -> TextureResource

Synchronously creates a 2D texture array by generating it from images.

convenience init(dimensions: TextureResource.Dimensions2DArray, format: TextureResource.Format, contents: TextureResource.Contents) async throws

Asynchronously creates a 2D array texture resource from a pixel Metal buffer, or data.

struct Dimensions2DArray

The dimensions of the 2D array texture.

