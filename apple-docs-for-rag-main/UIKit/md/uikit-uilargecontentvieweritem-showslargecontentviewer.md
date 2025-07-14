

- UIKit
- UILargeContentViewerItem
-  showsLargeContentViewer 

Instance Property

# showsLargeContentViewer

A Boolean value that indicates whether or not to show the item in the large content viewer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var showsLargeContentViewer: Bool { get }
```

**Required**

## Discussion

For this property to take effect, the item or an ancestor view must have a UILargeContentViewerInteraction.

