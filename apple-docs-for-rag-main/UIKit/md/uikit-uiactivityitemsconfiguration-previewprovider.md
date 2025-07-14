

- UIKit
- UIActivityItemsConfiguration
-  previewProvider 

Instance Property

# previewProvider

A closure that provides previews for the activity items.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var previewProvider: ((Int, UIActivityItemsConfigurationPreviewIntent, CGSize) -> NSItemProvider?)? { get set }
```

## See Also

### Managing previews

struct UIActivityItemsConfigurationPreviewIntent

A structure that specifies the types of activity item previews.

