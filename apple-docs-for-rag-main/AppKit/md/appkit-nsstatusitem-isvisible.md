

- AppKit
- NSStatusItem
-  isVisible 

Instance Property

# isVisible

A Boolean value indicating if the menu bar currently displays the status item.

macOS 10.12+

``` source
var isVisible: Bool { get set }
```

## Discussion

Setting this property either shows or hides the status item within the menu bar. The item’s visiblity may also change if the user removes the item manually, and you can watch for changes in visibility using key-value observation. The status item’s visiblity persists and restores automatically based on the value of autosaveName.

This property returns true even if the status item is temporarily hidden due to insufficient space in the menu bar. The default value is true.

## See Also

### Configuring the Status Item’s Appearance

var length: CGFloat

The amount of space in the status bar that should be allocated to the status item.

class let squareLength: CGFloat

A status item length that is equal to the status bar’s thickness.

class let variableLength: CGFloat

A status item length that dynamically adjusts to the width of its contents.

