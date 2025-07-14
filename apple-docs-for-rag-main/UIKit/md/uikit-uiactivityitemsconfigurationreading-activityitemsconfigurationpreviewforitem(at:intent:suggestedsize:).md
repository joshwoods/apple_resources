

- UIKit
- UIActivityItemsConfigurationReading
-  activityItemsConfigurationPreviewForItem(at:intent:suggestedSize:) 

Instance Method

# activityItemsConfigurationPreviewForItem(at:intent:suggestedSize:)

Returns an activity items configuration preview for the specified item and preview size.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func activityItemsConfigurationPreviewForItem(
    at index: Int,
    intent: UIActivityItemsConfigurationPreviewIntent,
    suggestedSize: CGSize
) -> NSItemProvider?
```

## See Also

### Managing Previews

struct UIActivityItemsConfigurationPreviewIntent

A structure that specifies the types of activity item previews.

