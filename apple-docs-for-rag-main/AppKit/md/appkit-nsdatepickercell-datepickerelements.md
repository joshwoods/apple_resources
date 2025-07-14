

- AppKit
- NSDatePickerCell
-  datePickerElements 

Instance Property

# datePickerElements

A bitmask that indicates which visual elements are shown by the date picker.

macOS

``` source
@MainActor
var datePickerElements: NSDatePicker.ElementFlags { get set }
```

## Discussion

Elements not included in the bitmask are hidden from view. For a list of possible values, see NSDatePicker.ElementFlags.

## See Also

### Configuring Appearance

var backgroundColor: NSColor

The cell’s background color.

var drawsBackground: Bool

A Boolean value indicating whether the cell draws its background.

var textColor: NSColor

The cell’s text color.

var datePickerStyle: NSDatePicker.Style

The date picker style to use.

