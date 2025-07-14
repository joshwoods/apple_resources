

- AppKit
- NSPreviewRepresentableActivityItem
-  iconProvider 

Instance Property

# iconProvider

An object that provides an icon that represents the item’s source.

macOS 13.0+

``` source
optional var iconProvider: NSItemProvider? { get }
```

## Discussion

Typically, the icon is a thumbnail-sized representation of the source app for the content. For example, provide your app’s icon for content you manage.

## See Also

### Providing Metadata About the Item

var title: String?

A localized string that contains the name of the item.

var imageProvider: NSItemProvider?

An object that provides a visual representation of the item.

