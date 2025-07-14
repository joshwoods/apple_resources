

- UIKit
-  UIPickerViewDelegate 

Protocol

# UIPickerViewDelegate

The interface for a picker view’s delegate.

iOSiPadOSMac CatalystvisionOS

``` source
@MainActor
protocol UIPickerViewDelegate : NSObjectProtocol
```

## Overview

The delegate of a UIPickerView object must adopt this protocol and implement at least some of its methods to provide the picker view with the data it needs to construct itself.

The delegate implements the required methods of this protocol to return height, width, row title, and the view content for the rows in each component. It must also provide the content for each component’s row, either as a string or a view. Typically the delegate implements other optional methods to respond to new selections or deselections of component rows.

See UIPickerView for a discussion of components, rows, row content, and row selection.

## Topics

### Setting the dimensions of the picker view

func pickerView(UIPickerView, rowHeightForComponent: Int) -> CGFloat

Called by the picker view when it needs the row height to use for drawing row content.

func pickerView(UIPickerView, widthForComponent: Int) -> CGFloat

Called by the picker view when it needs the row width to use for drawing row content.

### Setting the content of component rows

The methods in this group are marked `@optional`. However, to use a picker view, you must implement either the pickerView(_:titleForRow:forComponent:) or the pickerView(_:viewForRow:forComponent:reusing:) method to provide the content of component rows.

func pickerView(UIPickerView, titleForRow: Int, forComponent: Int) -> String?

Called by the picker view when it needs the title to use for a given row in a given component.

func pickerView(UIPickerView, attributedTitleForRow: Int, forComponent: Int) -> NSAttributedString?

Called by the picker view when it needs the styled title to use for a given row in a given component.

func pickerView(UIPickerView, viewForRow: Int, forComponent: Int, reusing: UIView?) -> UIView

Called by the picker view when it needs the view to use for a given row in a given component.

### Responding to row selection

func pickerView(UIPickerView, didSelectRow: Int, inComponent: Int)

Called by the picker view when the user selects a row in a component.

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- UIPickerViewAccessibilityDelegate

## See Also

### Customizing the picker behavior

var delegate: (any UIPickerViewDelegate)?

The delegate for the picker view.

