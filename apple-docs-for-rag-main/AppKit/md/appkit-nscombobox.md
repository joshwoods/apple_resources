

- AppKit
-  NSComboBox 

Class

# NSComboBox

A view that displays a list of values in a pop-up menu where the user selects a value or types in a custom value.

macOS

``` source
@MainActor
class NSComboBox
```

## Overview

A combo box combines the behavior of an NSTextField object with an NSPopUpButton object. A combo box displays a list of values from a pop-up list, but also provides a means for users to type in custom values. For example, here’s a combo box in its initial state.

Clicking in the text portion of the control allows the user to edit the current value. When the user clicks the down arrow at the right side of the text field, the pop-up list appears.

The NSComboBox class uses NSComboBoxCell to implement its user interface.

Also see the NSComboBoxDataSource protocol, which declares the methods that NSComboBox uses to access the contents of its data source object.

## Topics

### Setting Display Attributes

var hasVerticalScroller: Bool

A Boolean value indicating whether the combo box has a vertical scroller.

var intercellSpacing: NSSize

The horizontal and vertical spacing between cells in the pop-up list.

var isButtonBordered: Bool

A Boolean value indicating whether the combo box displays a border.

var itemHeight: CGFloat

The height of each item in the pop-up list.

var numberOfVisibleItems: Int

The maximum number of visible items to display in the pop-up list at one time.

### Setting a Data Source

var dataSource: (any NSComboBoxDataSource)?

The object that provides the item data for the combo box.

var usesDataSource: Bool

A Boolean value indicating whether the combo box retrieves its items from a data source object.

### Configuring the Combo Box Items

func addItems(withObjectValues: [Any])

Adds multiple objects to the end of the receiver’s internal item list.

func addItem(withObjectValue: Any)

Adds an object to the end of the receiver’s internal item list.

func insertItem(withObjectValue: Any, at: Int)

Inserts an object at the specified location in the receiver’s internal item list.

var objectValues: [Any]

An array of the items from the combo box’s internal list.

func removeAllItems()

Removes all items from the receiver’s internal item list.

func removeItem(at: Int)

Removes the object at the specified location from the receiver’s internal item list.

func removeItem(withObjectValue: Any)

Removes all occurrences of the given object from the receiver’s internal item list.

var numberOfItems: Int

The total number of items in the pop-up list.

### Manipulating the Displayed List

func indexOfItem(withObjectValue: Any) -> Int

Searches the receiver’s internal item list for the specified object and returns the lowest matching index.

func itemObjectValue(at: Int) -> Any

Returns the object located at the given index within the receiver’s internal item list.

func noteNumberOfItemsChanged()

Informs the receiver that the number of items in its data source has changed.

func reloadData()

Marks the receiver as needing redisplay, so that it will reload the data for visible pop-up items and draw the new values.

func scrollItemAtIndexToTop(Int)

Scrolls the receiver’s pop-up list vertically so that the item at the specified index is as close to the top as possible.

func scrollItemAtIndexToVisible(Int)

Scrolls the receiver’s pop-up list vertically so that the item at the specified index is visible.

### Manipulating the Selection

func deselectItem(at: Int)

Deselects the pop-up list item at the specified index if it’s selected.

var indexOfSelectedItem: Int

The index of the last item selected from the pop-up list.

var objectValueOfSelectedItem: Any?

The object corresponding to the last item selected from the pop-up list.

func selectItem(at: Int)

Selects the pop-up list row at the given index.

func selectItem(withObjectValue: Any?)

Selects the first pop-up list item that corresponds to the given object.

### Completing the Text Field

var completes: Bool

A Boolean value indicating whether the combo box tries to complete what the user types.

### Accessing the Delegate

var delegate: (any NSComboBoxDelegate)?

Sets the receiver’s delegate.

### Notifications

class let selectionDidChangeNotification: NSNotification.Name

Posted after the pop-up list selection of the `NSComboBox` changes.

class let selectionIsChangingNotification: NSNotification.Name

Posted whenever the pop-up list selection of the `NSComboBox` is changing.

class let willDismissNotification: NSNotification.Name

Posted whenever the pop-up list of the `NSComboBox` is about to be dismissed.

class let willPopUpNotification: NSNotification.Name

Posted whenever the pop-up list of the `NSComboBox` is going to be displayed.

## Relationships

### Inherits From

- NSTextField

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityNavigableStaticText
- NSAccessibilityProtocol
- NSAccessibilityStaticText
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTextContent
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- NSUserInterfaceValidations
- Sendable

