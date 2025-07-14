

- AppKit
- NSMenuItemCell
-  imageWidth 

Instance Property

# imageWidth

The width of the image associated with the menu item.

macOS

``` source
@MainActor
var imageWidth: CGFloat { get }
```

## Discussion

The width of the image is measured in points. You can associate an image with a menu item using the setImage: method of NSMenuItem.

## See Also

### Calculating the Size of a Menu Item

func calcSize()

Calculates the minimum required width and height of the receiver’s menu item.

var needsSizing: Bool

A Boolean value indicating whether the size of the menu needs to be calculated.

var titleWidth: CGFloat

The width of the menu item’s text, measured in points.

var keyEquivalentWidth: CGFloat

The width of the menu item’s key equivalent string.

var stateImageWidth: CGFloat

The width of the image used to indicate the state of the menu item.

