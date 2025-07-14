

- UIKit
-  UIDatePickerStyle 

Enumeration

# UIDatePickerStyle

Styles that determine the appearance of a date picker.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
enum UIDatePickerStyle
```

## Overview

A date picker style determines how your app displays the date picker value and its editor. For instance, a date picker with a datePickerMode of UIDatePicker.Mode.dateAndTime and datePickerStyle of UIDatePickerStyle.compact displays the date picker’s value as a label that the user can tap to view a calendar-style editor. On the other hand, the same date picker using the UIDatePickerStyle.inline style displays a view that lets the user edit the value without having to tap the label shown in the UIDatePickerStyle.compact style.

## Topics

### Styles

case automatic

A style indicating that the system picks the concrete style based on the current platform and date picker mode.

case compact

A style indicating that the date picker displays as a label that when tapped displays a calendar-style editor.

case inline

A style indicating that the date pickers displays as an inline, editable field.

case wheels

A style indicating that the date picker displays as a wheel picker.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring the date picker style

var datePickerStyle: UIDatePickerStyle

The current style of the date picker.

var preferredDatePickerStyle: UIDatePickerStyle

The preferred style of the date picker.

