

- AppKit
- NSDatePicker
-  presentsCalendarOverlay 

Instance Property

# presentsCalendarOverlay

A Boolean value that indicates whether to present a graphical calendar overlay when editing a calendar element within a text-field style date picker.

macOS 10.15.4+

``` source
@MainActor
var presentsCalendarOverlay: Bool { get set }
```

## Discussion

The default value is `NO`. The overlay only appears for text-style date pickers when you select a calendar element. The overlay doesn’t appear when there are no calendar events or the value of this property is `YES`.

## See Also

### Configuring Date Pickers

var isBezeled: Bool

A Boolean value that indicates whether the date picker draws a bezeled border.

var isBordered: Bool

A Boolean value that indicates whether the date picker has a plain border.

var backgroundColor: NSColor

The date picker’s background color.

var drawsBackground: Bool

A Boolean value that indicates whether the date picker draws the background.

var textColor: NSColor

The date picker’s text color.

var datePickerStyle: NSDatePicker.Style

The date picker’s style.

var delegate: (any NSDatePickerCellDelegate)?

A delegate for the date picker’s cell

var datePickerElements: NSDatePicker.ElementFlags

A bitmask that indicates which visual elements of the date picker are currently shown, and which won’t be usable because they are hidden.

struct ElementFlags

Constants that specify the date and time elements displayed by the picker.

enum Style

Constants that define the visual appearance of the date picker cell.

