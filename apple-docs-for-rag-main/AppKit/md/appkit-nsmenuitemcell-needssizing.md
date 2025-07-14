

- AppKit
- NSMenuItemCell
-  needsSizing 

Instance Property

# needsSizing

A Boolean value indicating whether the size of the menu needs to be calculated.

macOS

``` source
@MainActor
var needsSizing: Bool { get set }
```

## Discussion

When the value of this property is true, the next attempt to obtain size information about the menu cause the calcSize() method to be called. When the value of the property is false, the size information is obtained from the currently cached values.

Subclasses that drastically change the way a menu item is drawn can change the value of this property to update the menu item information. Other parts of your application should not need to change this property directly. The cell checks this value of this property as necessary when the content of its menu item changes.

## See Also

### Calculating the Size of a Menu Item

func calcSize()

Calculates the minimum required width and height of the receiver’s menu item.

var imageWidth: CGFloat

The width of the image associated with the menu item.

var titleWidth: CGFloat

The width of the menu item’s text, measured in points.

var keyEquivalentWidth: CGFloat

The width of the menu item’s key equivalent string.

var stateImageWidth: CGFloat

The width of the image used to indicate the state of the menu item.

