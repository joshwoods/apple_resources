

- AppKit
- NSMenuItemCell
-  calcSize() 

Instance Method

# calcSize()

Calculates the minimum required width and height of the receiver’s menu item.

macOS

``` source
@MainActor
func calcSize()
```

## Discussion

The calculated values are cached for future use. This method also calculates the sizes of individual components of the cell’s menu item and caches those values.

This method is invoked automatically when necessary. You should not need to invoke it directly.

## See Also

### Calculating the Size of a Menu Item

var needsSizing: Bool

A Boolean value indicating whether the size of the menu needs to be calculated.

var imageWidth: CGFloat

The width of the image associated with the menu item.

var titleWidth: CGFloat

The width of the menu item’s text, measured in points.

var keyEquivalentWidth: CGFloat

The width of the menu item’s key equivalent string.

var stateImageWidth: CGFloat

The width of the image used to indicate the state of the menu item.

