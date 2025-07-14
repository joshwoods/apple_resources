

- AppKit
-  NSDatePicker 

Class

# NSDatePicker

A display of a calendar date with controls for editing the date value.

macOS

``` source
@MainActor
class NSDatePicker
```

## Overview

`NSDatePicker` uses an NSDatePickerCell to implement much of the control’s functionality. `NSDatePicker` provides cover methods for most of `NSDatePickerCell` methods, which invoke the corresponding cell method.

## Topics

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

### Controlling Date Picker Range and Mode

var calendar: Calendar?

The calendar used by the date picker.

var locale: Locale?

The date picker’s locale.

var datePickerMode: NSDatePicker.Mode

The date picker’s mode.

var timeZone: TimeZone?

The time zone for the date picker.

enum Mode

Constants that define whether the picker provides a single date, or a range of dates.

### Accessing Object Values

var dateValue: Date

The date selected by the date picker.

var timeInterval: TimeInterval

The time interval selected by the date picker.

### Constraining the Displayable/Selectable Range

var minDate: Date?

The date picker’s minimum date value.

var maxDate: Date?

The date picker’s maximum date value.

## Relationships

### Inherits From

- NSControl

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable

