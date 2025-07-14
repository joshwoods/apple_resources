

- AppKit
- NSDatePicker
-  isBordered 

Instance Property

# isBordered

A Boolean value that indicates whether the date picker has a plain border.

macOS

``` source
@MainActor
var isBordered: Bool { get set }
```

## Discussion

This property contains true if the date picker has a plain boarder; otherwise, false.

## See Also

### Configuring Date Pickers

var isBezeled: Bool

A Boolean value that indicates whether the date picker draws a bezeled border.

var backgroundColor: NSColor

The date picker’s background color.

var drawsBackground: Bool

A Boolean value that indicates whether the date picker draws the background.

var textColor: NSColor

The date picker’s text color.

var datePickerStyle: NSDatePicker.Style

The date picker’s style.

var presentsCalendarOverlay: Bool

A Boolean value that indicates whether to present a graphical calendar overlay when editing a calendar element within a text-field style date picker.

var delegate: (any NSDatePickerCellDelegate)?

A delegate for the date picker’s cell

var datePickerElements: NSDatePicker.ElementFlags

A bitmask that indicates which visual elements of the date picker are currently shown, and which won’t be usable because they are hidden.

struct ElementFlags

Constants that specify the date and time elements displayed by the picker.

enum Style

Constants that define the visual appearance of the date picker cell.

