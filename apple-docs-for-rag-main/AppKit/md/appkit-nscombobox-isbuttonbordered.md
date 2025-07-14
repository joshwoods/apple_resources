

- AppKit
- NSComboBox
-  isButtonBordered 

Instance Property

# isButtonBordered

A Boolean value indicating whether the combo box displays a border.

macOS

``` source
@MainActor
var isButtonBordered: Bool { get set }
```

## Discussion

When the value of this property is true, the combo box displays a border. For example, when displaying a combo box in a table, it is often useful to display the combo box without a border. The default value of this property is true.

## See Also

### Setting Display Attributes

var hasVerticalScroller: Bool

A Boolean value indicating whether the combo box has a vertical scroller.

var intercellSpacing: NSSize

The horizontal and vertical spacing between cells in the pop-up list.

var itemHeight: CGFloat

The height of each item in the pop-up list.

var numberOfVisibleItems: Int

The maximum number of visible items to display in the pop-up list at one time.

