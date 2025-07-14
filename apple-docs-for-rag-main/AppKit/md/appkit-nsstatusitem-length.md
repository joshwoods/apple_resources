

- AppKit
- NSStatusItem
-  length 

Instance Property

# length

The amount of space in the status bar that should be allocated to the status item.

macOS

``` source
var length: CGFloat { get set }
```

## Discussion

If the status bar is horizontal, the value of this property is the width of the status item. In addition to a fixed length, this value can be NSSquareStatusItemLength or NSVariableStatusItemLength (see `NSStatusBar` Constants) to allow the status bar to allocate (and adjust) the space according to either the status bar’s thickness or the status item’s true size.

## See Also

### Configuring the Status Item’s Appearance

var isVisible: Bool

A Boolean value indicating if the menu bar currently displays the status item.

class let squareLength: CGFloat

A status item length that is equal to the status bar’s thickness.

class let variableLength: CGFloat

A status item length that dynamically adjusts to the width of its contents.

