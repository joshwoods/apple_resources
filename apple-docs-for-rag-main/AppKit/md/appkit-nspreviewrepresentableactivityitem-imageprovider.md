

- AppKit
- NSPreviewRepresentableActivityItem
-  imageProvider 

Instance Property

# imageProvider

An object that provides a visual representation of the item.

macOS 13.0+

``` source
optional var imageProvider: NSItemProvider? { get }
```

## Discussion

Provide a full-size representation of the content you’re sharing. For example, if the shared item is a link to a webpage, provide the hero image for that webpage or a rendering of the page.

## See Also

### Providing Metadata About the Item

var title: String?

A localized string that contains the name of the item.

var iconProvider: NSItemProvider?

An object that provides an icon that represents the item’s source.

