

- AppKit
- NSComboBoxCell
-  intercellSpacing 

Instance Property

# intercellSpacing

The spacing between cells in the combo box’s pop-up list.

macOS

``` source
@MainActor
var intercellSpacing: NSSize { get set }
```

## Discussion

The value of this property is the horizontal and vertical spacing between cells in the combo box’s pop-up list. The default spacing is (3.0, 2.0).

## See Also

### Setting Display Attributes

var hasVerticalScroller: Bool

A Boolean value that indicates if the combo box displays a vertical scroller.

var isButtonBordered: Bool

A Boolean value that indicates whether the combo box button displays a border.

var itemHeight: CGFloat

The height of each item in the combo box’s pop-up list.

var numberOfVisibleItems: Int

The maximum number of items visible in the pop-up list at any one time.

