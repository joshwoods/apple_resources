

- RealityKit
- EnvironmentResource
-  init(named:in:) 

Initializer

# init(named:in:)

Asynchronously loads an environment resource from a bundle.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
convenience init(
    named name: String,
    in bundle: Bundle? = nil
) async throws
```

## See Also

### Loading the resource

convenience init(equirectangular: CGImage, withName: String?) throws

Synchronously creates an environment resource from an equirectangular image.

convenience init(equirectangular: CGImage, withName: String?) async throws

Asynchronously generates an environment resource from an equirectangular image.

convenience init(cube: TextureResource, options: EnvironmentResource.CreateOptions) async throws

Asynchronously creates an environment resource from a cube texture.

convenience init(cube: TextureResource, options: EnvironmentResource.CreateOptions) throws

Synchronously generates an environment resource from a cube texture resource.

static func load(named: String, in: Bundle?) throws -> EnvironmentResource

Synchronously loads an environment resource from a bundle.

