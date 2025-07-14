

- AppKit
- NSComboBox
-  intercellSpacing 

Instance Property

# intercellSpacing

The horizontal and vertical spacing between cells in the pop-up list.

macOS

``` source
@MainActor
var intercellSpacing: NSSize { get set }
```

## Discussion

Spacing values are measured in points. The default spacing is (`3.0`, `2.0`).

## See Also

### Setting Display Attributes

var hasVerticalScroller: Bool

A Boolean value indicating whether the combo box has a vertical scroller.

var isButtonBordered: Bool

A Boolean value indicating whether the combo box displays a border.

var itemHeight: CGFloat

The height of each item in the pop-up list.

var numberOfVisibleItems: Int

The maximum number of visible items to display in the pop-up list at one time.

