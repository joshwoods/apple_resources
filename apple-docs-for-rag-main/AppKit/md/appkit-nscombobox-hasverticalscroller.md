

- AppKit
- NSComboBox
-  hasVerticalScroller 

Instance Property

# hasVerticalScroller

A Boolean value indicating whether the combo box has a vertical scroller.

macOS

``` source
@MainActor
var hasVerticalScroller: Bool { get set }
```

## Discussion

When the value of this property is true, the combo box displays a vertical scroller even when the pop-up list contains few enough items that a scroller is not needed. The default value of this property is true.

If the value of this property is false and the combo box has more list items (either in its internal item list or from its data source) than are allowed by numberOfVisibleItems, only a subset of items are displayed. The `NSComboBox` class’ `scroll...` methods can be used to position this subset within the pop-up list.

## See Also

### Related Documentation

var numberOfItems: Int

The total number of items in the pop-up list.

func scrollItemAtIndexToTop(Int)

Scrolls the receiver’s pop-up list vertically so that the item at the specified index is as close to the top as possible.

Combo Box Programming Topics

func scrollItemAtIndexToVisible(Int)

Scrolls the receiver’s pop-up list vertically so that the item at the specified index is visible.

### Setting Display Attributes

var intercellSpacing: NSSize

The horizontal and vertical spacing between cells in the pop-up list.

var isButtonBordered: Bool

A Boolean value indicating whether the combo box displays a border.

var itemHeight: CGFloat

The height of each item in the pop-up list.

var numberOfVisibleItems: Int

The maximum number of visible items to display in the pop-up list at one time.

