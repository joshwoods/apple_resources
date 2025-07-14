

- AppKit
- NSComboBox
-  itemHeight 

Instance Property

# itemHeight

The height of each item in the pop-up list.

macOS

``` source
@MainActor
var itemHeight: CGFloat { get set }
```

## Discussion

The height of items is measured in points. The default item height is `16.0` points.

## See Also

### Setting Display Attributes

var hasVerticalScroller: Bool

A Boolean value indicating whether the combo box has a vertical scroller.

var intercellSpacing: NSSize

The horizontal and vertical spacing between cells in the pop-up list.

var isButtonBordered: Bool

A Boolean value indicating whether the combo box displays a border.

var numberOfVisibleItems: Int

The maximum number of visible items to display in the pop-up list at one time.

