

- DeveloperToolsSupport
- PreviewTrait
-  defaultLayout 

Type Property

# defaultLayout

Center the preview in a container the size of the device on which the preview is running.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor
static var defaultLayout: PreviewTrait { get }
```

Available when `T` is `Preview.ViewTraits`.

## Discussion

This is the same as the PreviewLayout.device layout, and is the default if you don’t specify a layout trait.

