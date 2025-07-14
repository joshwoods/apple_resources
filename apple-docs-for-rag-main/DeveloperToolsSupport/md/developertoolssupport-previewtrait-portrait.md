

- DeveloperToolsSupport
- PreviewTrait
-  portrait 

Type Property

# portrait

The device is in portrait mode, with the top of the device on top.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor
static var portrait: PreviewTrait { get }
```

Available when `T` is `Preview.ViewTraits`.

## Discussion

This is the same as portrait and is the default orientation if you don’t specify one.

