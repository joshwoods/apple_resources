

- AppKit
- NSDatePickerCell
-  drawsBackground 

Instance Property

# drawsBackground

A Boolean value indicating whether the cell draws its background.

macOS

``` source
@MainActor
var drawsBackground: Bool { get set }
```

## Discussion

When the value of this property is true, the cell draws its background.

## See Also

### Configuring Appearance

var backgroundColor: NSColor

The cell’s background color.

var textColor: NSColor

The cell’s text color.

var datePickerStyle: NSDatePicker.Style

The date picker style to use.

var datePickerElements: NSDatePicker.ElementFlags

A bitmask that indicates which visual elements are shown by the date picker.

