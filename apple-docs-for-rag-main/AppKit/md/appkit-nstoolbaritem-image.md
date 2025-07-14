

- AppKit
- NSToolbarItem
-  image 

Instance Property

# image

The image to display for the toolbar item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

**Mac Catalyst**

``` source
@MainActor
var image: UIImage? { get set }
```

**macOS**

``` source
@MainActor
var image: NSImage? { get set }
```

## Discussion

If you assign a custom view to the toolbar item, modifying this property updates the `image` property of the view, if one exists. If the item doesn’t contain a custom view, the toolbar item manages the image content directly.

## See Also

### Getting the item’s visual appearance

var view: NSView?

The custom view you use to draw the toolbar item.

