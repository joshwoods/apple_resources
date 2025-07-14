

- UIKit
- UIActivityItemsConfigurationProviding
-  activityItemsConfiguration 

Instance Property

# activityItemsConfiguration

An object or value that specifies items to share.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
var activityItemsConfiguration: (any UIActivityItemsConfigurationReading)? { get }
```

**Required**

## Discussion

To offer a configuration for sharing through Siri or the toolbar in an app built with Mac Catalyst, override this property on the root view controller or a modal view controller. To provide a configuration when your app is displaying a UISplitViewController, implement this property on the detail view controller.

To offer a configuration for sharing through a context menu, override this property on your UIView subclass, and attach a UIContextMenuInteraction to that view.

Note

When the user asks Siri to “share this” on iOS, if both activityItemsConfiguration and activityItemsConfigurationSource are `nil`, the system uses the webpageURL property on your app’s current userActivity to create shareable content. The system doesn’t offer this fallback behavior in an app built with Mac Catalyst.

