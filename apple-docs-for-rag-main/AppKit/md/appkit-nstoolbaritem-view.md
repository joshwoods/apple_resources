

- AppKit
- NSToolbarItem
-  view 

Instance Property

# view

The custom view you use to draw the toolbar item.

macOS

``` source
@MainActor
var view: NSView? { get set }
```

## Discussion

Many properties of NSToolbarItem automatically forward changes to the associated custom NSView object, if the view has a property or accessor method with a matching name.

## See Also

### Getting the item’s visual appearance

var image: UIImage?

The image to display for the toolbar item.

