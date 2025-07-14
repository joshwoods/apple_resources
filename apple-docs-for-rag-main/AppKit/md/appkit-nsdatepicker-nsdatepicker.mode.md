

- AppKit
- NSDatePicker
-  NSDatePicker.Mode 

Enumeration

# NSDatePicker.Mode

Constants that define whether the picker provides a single date, or a range of dates.

macOS

``` source
enum Mode
```

## Topics

### Enumeration Cases

case range

case single

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Controlling Date Picker Range and Mode

var calendar: Calendar?

The calendar used by the date picker.

var locale: Locale?

The date picker’s locale.

var datePickerMode: NSDatePicker.Mode

The date picker’s mode.

var timeZone: TimeZone?

The time zone for the date picker.

