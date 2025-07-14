

- AppKit
-  NSComboBoxCell 

Class

# NSComboBoxCell

The user interface of a combo box.

macOS

``` source
@MainActor
class NSComboBoxCell
```

## Overview

NSComboBoxCell is a subclass of NSTextFieldCell used to implement the user interface of “combo boxes” (see NSComboBox for information on how combo boxes look and work). The NSComboBox subclass of NSTextField uses a single NSComboBoxCell, and essentially all of the NSComboBox class’s methods simply invoke the corresponding NSComboBoxCell method.

Also see the NSComboBoxCellDataSource protocol, which declares the methods that an NSComboBoxCell object uses to access the contents of its data source object.

## Topics

### Setting Display Attributes

var hasVerticalScroller: Bool

A Boolean value that indicates if the combo box displays a vertical scroller.

var isButtonBordered: Bool

A Boolean value that indicates whether the combo box button displays a border.

var intercellSpacing: NSSize

The spacing between cells in the combo box’s pop-up list.

var itemHeight: CGFloat

The height of each item in the combo box’s pop-up list.

var numberOfVisibleItems: Int

The maximum number of items visible in the pop-up list at any one time.

### Accessing a Data Source

var dataSource: (any NSComboBoxCellDataSource)?

The object that provides the data displayed in the combo box’s pop-up list.

var usesDataSource: Bool

A Boolean value that indicates if the combo box uses an external data source to populate its pop-up list.

### Working with an Internal List

func addItems(withObjectValues: [Any])

Adds multiple objects to the internal item list.

func addItem(withObjectValue: Any)

Adds the specified object to the internal item list.

func insertItem(withObjectValue: Any, at: Int)

Inserts an object at the specified location in the internal item list.

var objectValues: [Any]

The combo box’s internal item list in an array.

func removeAllItems()

Removes all items from the combo box’s internal item list.

func removeItem(at: Int)

Removes the object at the specified location from the combo box’s internal item list.

func removeItem(withObjectValue: Any)

Removes all occurrences of the specified object from the combo box’s internal item list.

var numberOfItems: Int

The total number of items in the pop-up list.

### Manipulating the Displayed List

func indexOfItem(withObjectValue: Any) -> Int

Searches the combo box’s internal item list for the given object and returns the matching index number.

func itemObjectValue(at: Int) -> Any

Returns the object located at the specified location in the internal item list.

func noteNumberOfItemsChanged()

Informs the combo box that the number of items in its data source has changed.

func reloadData()

Marks the combo box as needing redisplay, so that it will reload the data for visible pop-up items and draw the new values.

func scrollItemAtIndexToTop(Int)

Scrolls the combo box’s pop-up list vertically so that the item at the given index is as close to the top as possible.

func scrollItemAtIndexToVisible(Int)

Scrolls the combo box’s pop-up list vertically so that the item at the given index is visible.

### Manipulating the Selection

func deselectItem(at: Int)

Deselects the pop-up list item at the given index if it’s selected.

var indexOfSelectedItem: Int

The index of the last item selected from the pop-up list.

var objectValueOfSelectedItem: Any?

The object corresponding to the last item selected from the pop-up list.

func selectItem(at: Int)

Selects the pop-up list row at the given index.

func selectItem(withObjectValue: Any?)

Selects the first pop-up list item that corresponds to the specified object.

### Completing the Text Field

func completedString(String) -> String?

Returns a string from the combo box’s pop-up list that starts with the given substring.

var completes: Bool

A Boolean value that indicates if the combo box tries to complete text entered by the user.

## Relationships

### Inherits From

- NSTextFieldCell

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSCoding
- NSCopying
- NSObjectProtocol
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Cells

protocol NSComboBoxCellDataSource

