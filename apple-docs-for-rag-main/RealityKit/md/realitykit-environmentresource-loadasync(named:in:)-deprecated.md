

- RealityKit
- EnvironmentResource
-  loadAsync(named:in:) Deprecated

Type Method

# loadAsync(named:in:)

Asynchronously loads an environment resource from a bundle.

iOS 13.0–18.0DeprecatediPadOS 13.0–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 10.15–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor @preconcurrency
static func loadAsync(
    named name: String,
    in bundle: Bundle? = nil
) -> LoadRequest
```

## Parameters 

`name`  

The image name without the file extension.

`bundle`  

The bundle to search for the resource. Use `nil` to indicate the app’s bundle.

## Return Value

The environment resource that loads from the specified bundle.

## Discussion

If your image file is at the path `Foo.skybox/Bar.exr` in your Xcode project, use `Bar` for the name parameter. You need to call this function with the `async` keyword from an asynchronous context, such as from within a Task closure.

To add an environment resource to your Xcode project, see EnvironmentResource.

## See Also

### Deprecated

static func generate(fromEquirectangular: CGImage, withName: String?) throws -> EnvironmentResource

Synchronously generates an environment resource from an equirectangular image.

Deprecated

static func generate(fromEquirectangular: CGImage, withName: String?) async throws -> EnvironmentResource

Asynchronously generates an environment resource from an equirectangular image.

Deprecated

