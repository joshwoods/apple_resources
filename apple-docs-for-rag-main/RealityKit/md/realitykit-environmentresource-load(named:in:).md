

- RealityKit
- EnvironmentResource
-  load(named:in:) 

Type Method

# load(named:in:)

Synchronously loads an environment resource from a bundle.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
static func load(
    named name: String,
    in bundle: Bundle? = nil
) throws -> EnvironmentResource
```

## Parameters 

`name`  

The image name without the file extension.

`bundle`  

The bundle to search for the resource. Use `nil` to indicate the app’s bundle.

## Return Value

The environment resource that loads from the specified bundle.

## Discussion

Loading an EnvironmentResource with this method blocks the main actor because it’s synchronous, so only call it from a command-line application. The method can stall a regular app, which makes it visibly hitch, and the system terminates an app if its UI becomes unresponsive.

If your image file is at the path `Foo.skybox/Bar.exr` in your Xcode project, use `Bar` for the name parameter.

To add an environment resource to your Xcode project, see EnvironmentResource.

Important

This function blocks the calling thread while RealityKit loads the requested resource.

## See Also

### Loading the resource

convenience init(named: String, in: Bundle?) async throws

Asynchronously loads an environment resource from a bundle.

convenience init(equirectangular: CGImage, withName: String?) throws

Synchronously creates an environment resource from an equirectangular image.

convenience init(equirectangular: CGImage, withName: String?) async throws

Asynchronously generates an environment resource from an equirectangular image.

convenience init(cube: TextureResource, options: EnvironmentResource.CreateOptions) async throws

Asynchronously creates an environment resource from a cube texture.

convenience init(cube: TextureResource, options: EnvironmentResource.CreateOptions) throws

Synchronously generates an environment resource from a cube texture resource.

