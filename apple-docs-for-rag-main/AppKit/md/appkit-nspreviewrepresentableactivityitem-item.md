

- AppKit
- NSPreviewRepresentableActivityItem
-  item 

Instance Property

# item

The app-specific item you want to share.

macOS 13.0+

``` source
var item: Any { get }
```

**Required**

## Discussion

Use this property to provide the data you want to pass to the sharing service. The item must conform to the NSPasteboardWriting protocol, or be an NSItemProvider or NSDocument object.

