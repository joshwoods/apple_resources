

- AppKit
- NSDatePicker
-  NSDatePicker.ElementFlags 

Structure

# NSDatePicker.ElementFlags

Constants that specify the date and time elements displayed by the picker.

macOS

``` source
struct ElementFlags
```

## Overview

You can combine these constants using the C bitwise `OR` operator.

## Topics

### Constants

static var era: NSDatePicker.ElementFlags

static var hourMinute: NSDatePicker.ElementFlags

static var hourMinuteSecond: NSDatePicker.ElementFlags

static var timeZone: NSDatePicker.ElementFlags

static var yearMonth: NSDatePicker.ElementFlags

static var yearMonthDay: NSDatePicker.ElementFlags

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

var presentsCalendarOverlay: Bool

A Boolean value that indicates whether to present a graphical calendar overlay when editing a calendar element within a text-field style date picker.

var delegate: (any NSDatePickerCellDelegate)?

A delegate for the date picker’s cell

var datePickerElements: NSDatePicker.ElementFlags

A bitmask that indicates which visual elements of the date picker are currently shown, and which won’t be usable because they are hidden.

enum Style

Constants that define the visual appearance of the date picker cell.

