

- AppKit
- NSMenuItemCell
-  titleWidth 

Instance Property

# titleWidth

The width of the menu item’s text, measured in points.

macOS

``` source
@MainActor
var titleWidth: CGFloat { get }
```

## Discussion

To set the menu item’s text, use the setTitle: method of NSMenuItem.

## See Also

### Calculating the Size of a Menu Item

func calcSize()

Calculates the minimum required width and height of the receiver’s menu item.

var needsSizing: Bool

A Boolean value indicating whether the size of the menu needs to be calculated.

var imageWidth: CGFloat

The width of the image associated with the menu item.

var keyEquivalentWidth: CGFloat

The width of the menu item’s key equivalent string.

var stateImageWidth: CGFloat

The width of the image used to indicate the state of the menu item.

