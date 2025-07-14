

- SwiftUI
- View
-  datePickerStyle(\_:) 

Instance Method

# datePickerStyle(\_:)

Sets the style for date pickers within this view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func datePickerStyle(_ style: S) -> some View where S : DatePickerStyle
```

## See Also

### Choosing dates

struct DatePicker

A control for selecting an absolute date.

struct MultiDatePicker

A control for picking multiple dates.

var calendar: Calendar

The current calendar that views should use when handling dates.

var timeZone: TimeZone

The current time zone that views should use when handling dates.

