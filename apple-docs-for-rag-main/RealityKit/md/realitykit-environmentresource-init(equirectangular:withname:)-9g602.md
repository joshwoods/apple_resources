

- RealityKit
- EnvironmentResource
-  init(equirectangular:withName:) 

Initializer

# init(equirectangular:withName:)

Synchronously creates an environment resource from an equirectangular image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
convenience init(
    equirectangular cgImage: CGImage,
    withName resourceName: String? = nil
) throws
```

## Parameters 

`cgImage`  

The source equirectangular (latitude, longitude) image. To preserve all details use an image where the width is half the height.

`resourceName`  

A unique name the method assigns to the resource it loads, for use in network synchronization.

## Discussion

Loading an EnvironmentResource with this method blocks the main actor because it’s synchronous, so only call it from a command-line application. The method can stall a regular app, which makes it visibly hitch, and the system terminates an app if its UI becomes unresponsive.

## See Also

### Loading the resource

convenience init(named: String, in: Bundle?) async throws

Asynchronously loads an environment resource from a bundle.

convenience init(equirectangular: CGImage, withName: String?) async throws

Asynchronously generates an environment resource from an equirectangular image.

convenience init(cube: TextureResource, options: EnvironmentResource.CreateOptions) async throws

Asynchronously creates an environment resource from a cube texture.

convenience init(cube: TextureResource, options: EnvironmentResource.CreateOptions) throws

Synchronously generates an environment resource from a cube texture resource.

static func load(named: String, in: Bundle?) throws -> EnvironmentResource

Synchronously loads an environment resource from a bundle.

