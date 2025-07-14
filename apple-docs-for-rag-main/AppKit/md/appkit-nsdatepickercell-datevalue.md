

- AppKit
- NSDatePickerCell
-  dateValue 

Instance Property

# dateValue

The date currently specified in the picker.

macOS

``` source
@MainActor
var dateValue: Date { get set }
```

## Discussion

Assign a date to this property to set the starting value for the picker. For range-based dates, use the timeInterval property to set the extent of the time range.

## See Also

### Object Values

var timeInterval: TimeInterval

The time interval that represents the date range.

var calendar: Calendar?

The calendar used by the date picker.

var locale: Locale?

The locale used to display dates.

var timeZone: TimeZone?

The time zone used to display time-related values.

