

- SwiftUI
- PreviewProvider
-  platform 

Type Property

# platform

The platform on which to run the provider.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
static var platform: PreviewPlatform? { get }
```

**Required** Default implementation provided.

## Discussion

Xcode infers the platform for a preview based on the currently selected target. If you have a multiplatform target and want to suggest a particular target for a preview, implement the `platform` computed property to provide a hint, and specify one of the PreviewPlatform values:

```
struct CircleImage_Previews: PreviewProvider {
    static var previews: some View {
        CircleImage()
    }

    static var platform: PreviewPlatform? {
        PreviewPlatform.tvOS
    }
}
```

Xcode ignores this value unless you have a multiplatform target.

## Default Implementations

### PreviewProvider Implementations

static var platform: PreviewPlatform?

The platform to run the provider on.

