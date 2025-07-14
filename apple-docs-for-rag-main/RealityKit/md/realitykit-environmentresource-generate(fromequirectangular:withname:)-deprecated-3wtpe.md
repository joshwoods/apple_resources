

- RealityKit
- EnvironmentResource
-  generate(fromEquirectangular:withName:) Deprecated

Type Method

# generate(fromEquirectangular:withName:)

Synchronously generates an environment resource from an equirectangular image.

visionOS 1.0–2.0Deprecated

``` source
@MainActor @preconcurrency
static func generate(
    fromEquirectangular cgImage: CGImage,
    withName resourceName: String? = nil
) throws -> EnvironmentResource
```

## See Also

### Deprecated

static func generate(fromEquirectangular: CGImage, withName: String?) async throws -> EnvironmentResource

Asynchronously generates an environment resource from an equirectangular image.

Deprecated

static func loadAsync(named: String, in: Bundle?) -> LoadRequest&lt;EnvironmentResource>

Asynchronously loads an environment resource from a bundle.

Deprecated

