

- AppKit
- NSComboBoxCell
-  hasVerticalScroller 

Instance Property

# hasVerticalScroller

A Boolean value that indicates if the combo box displays a vertical scroller.

macOS

``` source
@MainActor
var hasVerticalScroller: Bool { get set }
```

## Discussion

When the value of this property is true, the combo box displays a vertical scroller; when the value is false, it does not. The default value of this property is true. Note that the scroller is displayed even if the pop-up list contains fewer items than will fit in the area specified for display.

If you set this property to false and the combo box cell has more list items (either in its internal item list or from its data source) than are allowed by numberOfVisibleItems, only a subset are displayed. The NSComboBoxCell `scroll...` methods can be used to position this subset within the pop-up list.

## See Also

### Related Documentation

Combo Box Programming Topics

func scrollItemAtIndexToTop(Int)

Scrolls the combo box’s pop-up list vertically so that the item at the given index is as close to the top as possible.

var numberOfItems: Int

The total number of items in the pop-up list.

func scrollItemAtIndexToVisible(Int)

Scrolls the combo box’s pop-up list vertically so that the item at the given index is visible.

### Setting Display Attributes

var isButtonBordered: Bool

A Boolean value that indicates whether the combo box button displays a border.

var intercellSpacing: NSSize

The spacing between cells in the combo box’s pop-up list.

var itemHeight: CGFloat

The height of each item in the combo box’s pop-up list.

var numberOfVisibleItems: Int

The maximum number of items visible in the pop-up list at any one time.

