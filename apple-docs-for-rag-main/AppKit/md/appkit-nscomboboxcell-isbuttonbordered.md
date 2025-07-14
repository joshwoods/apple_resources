

- AppKit
- NSComboBoxCell
-  isButtonBordered 

Instance Property

# isButtonBordered

A Boolean value that indicates whether the combo box button displays a border.

macOS

``` source
@MainActor
var isButtonBordered: Bool { get set }
```

## Discussion

When the value of this property is true, the button has a border; when it is false, the button is borderless. For example, it is often useful when using a combo box in an NSTableView to display the button without a border.

## See Also

### Setting Display Attributes

var hasVerticalScroller: Bool

A Boolean value that indicates if the combo box displays a vertical scroller.

var intercellSpacing: NSSize

The spacing between cells in the combo box’s pop-up list.

var itemHeight: CGFloat

The height of each item in the combo box’s pop-up list.

var numberOfVisibleItems: Int

The maximum number of items visible in the pop-up list at any one time.

