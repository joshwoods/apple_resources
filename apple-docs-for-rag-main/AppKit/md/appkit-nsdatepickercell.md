

- AppKit
-  NSDatePickerCell 

Class

# NSDatePickerCell

An object that controls the behavior of a date picker, or of a single date picker cell in a matrix.

macOS

``` source
@MainActor
class NSDatePickerCell
```

## Topics

### Configuring Appearance

var backgroundColor: NSColor

The cell’s background color.

var drawsBackground: Bool

A Boolean value indicating whether the cell draws its background.

var textColor: NSColor

The cell’s text color.

var datePickerStyle: NSDatePicker.Style

The date picker style to use.

var datePickerElements: NSDatePicker.ElementFlags

A bitmask that indicates which visual elements are shown by the date picker.

### Range Mode

var datePickerMode: NSDatePicker.Mode

The mode in use by the date picker.

### Object Values

var dateValue: Date

The date currently specified in the picker.

var timeInterval: TimeInterval

The time interval that represents the date range.

var calendar: Calendar?

The calendar used by the date picker.

var locale: Locale?

The locale used to display dates.

var timeZone: TimeZone?

The time zone used to display time-related values.

### Date Range Constraints

var minDate: Date?

The minimum date that the picker allows as input.

var maxDate: Date?

The maximum date that the picker allows as input.

### Getting and Setting the Delegate

var delegate: (any NSDatePickerCellDelegate)?

The delegate associated with the date picker.

### Constants

enum Style

Constants that define the visual appearance of the date picker cell.

enum Mode

Constants that define whether the picker provides a single date, or a range of dates.

struct ElementFlags

Constants that specify the date and time elements displayed by the picker.

### Initializers

init(coder: NSCoder)

init(textCell: String)

## Relationships

### Inherits From

- NSActionCell

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

protocol NSDatePickerCellDelegate

A set of optional methods implemented by delegates of NSDatePickerCell objects.

