

- AppKit
- NSDatePickerCell
-  timeInterval 

Instance Property

# timeInterval

The time interval that represents the date range.

macOS

``` source
@MainActor
var timeInterval: TimeInterval { get set }
```

## Discussion

The date range begins at the date in the dateValue property. The value in this property applies only when the date picker is in the NSRangeDateMode mode.

## See Also

### Object Values

var dateValue: Date

The date currently specified in the picker.

var calendar: Calendar?

The calendar used by the date picker.

var locale: Locale?

The locale used to display dates.

var timeZone: TimeZone?

The time zone used to display time-related values.

