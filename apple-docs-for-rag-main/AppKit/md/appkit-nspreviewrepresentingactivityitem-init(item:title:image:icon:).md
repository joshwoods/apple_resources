

- AppKit
- NSPreviewRepresentingActivityItem
-  init(item:title:image:icon:) 

Initializer

# init(item:title:image:icon:)

Creates a metadata object with the title, image, and icon for a shareable item.

macOS 13.0+

``` source
convenience init(
    item: Any,
    title: String?,
    image: NSImage?,
    icon: NSImage?
)
```

## Parameters 

`item`  

The item to share from the Mac share sheet. The item must conform to the NSPasteboardWriting protocol, or be an NSItemProvider or NSDocument object.

`title`  

The localized name of the item.

`image`  

An image to display as a preview for the item. For example, when you share a URL for a webpage, you might specify the hero image for that page or a rendering of the webpage itself.

`icon`  

A thumbnail-size image of the source of the item. Typically, you specify your app’s icon but you can provide a different icon if the content has a different source.

## Return Value

An initialized item to share.

## See Also

### Creating a Preview Activity Item

init(item: Any, title: String?, imageProvider: NSItemProvider?, iconProvider: NSItemProvider?)

Creates a metadata object that provides a title and images for a shareable item.

