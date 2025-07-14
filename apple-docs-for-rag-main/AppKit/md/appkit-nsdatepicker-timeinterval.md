

- AppKit
- NSDatePicker
-  timeInterval 

Instance Property

# timeInterval

The time interval selected by the date picker.

macOS

``` source
@MainActor
var timeInterval: TimeInterval { get set }
```

## Discussion

The time interval that represents the receiver’s date range. The date range begins at the date returned by dateValue. This method returns 0 when the receiver is not in the NSRangeDateMode mode.

## See Also

### Accessing Object Values

var dateValue: Date

The date selected by the date picker.

