

- AppKit
- NSMenuItemCell
-  keyEquivalentWidth 

Instance Property

# keyEquivalentWidth

The width of the menu item’s key equivalent string.

macOS

``` source
@MainActor
var keyEquivalentWidth: CGFloat { get }
```

## Discussion

To set the menu item’s key equivalent, use the keyEquivalent property of NSMenuItem.

## See Also

### Calculating the Size of a Menu Item

func calcSize()

Calculates the minimum required width and height of the receiver’s menu item.

var needsSizing: Bool

A Boolean value indicating whether the size of the menu needs to be calculated.

var imageWidth: CGFloat

The width of the image associated with the menu item.

var titleWidth: CGFloat

The width of the menu item’s text, measured in points.

var stateImageWidth: CGFloat

The width of the image used to indicate the state of the menu item.

