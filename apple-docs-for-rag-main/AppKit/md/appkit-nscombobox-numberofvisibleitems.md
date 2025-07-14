

- AppKit
- NSComboBox
-  numberOfVisibleItems 

Instance Property

# numberOfVisibleItems

The maximum number of visible items to display in the pop-up list at one time.

macOS

``` source
@MainActor
var numberOfVisibleItems: Int { get set }
```

## Discussion

Use this property to configure how many items can be displayed at the same time. If the combo box has a scroller, the user can scroll to view additional items beyond the visible range.

## See Also

### Related Documentation

var numberOfItems: Int

The total number of items in the pop-up list.

### Setting Display Attributes

var hasVerticalScroller: Bool

A Boolean value indicating whether the combo box has a vertical scroller.

var intercellSpacing: NSSize

The horizontal and vertical spacing between cells in the pop-up list.

var isButtonBordered: Bool

A Boolean value indicating whether the combo box displays a border.

var itemHeight: CGFloat

The height of each item in the pop-up list.

