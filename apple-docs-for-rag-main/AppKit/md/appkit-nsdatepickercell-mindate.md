

- AppKit
- NSDatePickerCell
-  minDate 

Instance Property

# minDate

The minimum date that the picker allows as input.

macOS

``` source
@MainActor
var minDate: Date? { get set }
```

## Discussion

Set this property to `nil` if you want to allow any value for the minimum date.

## See Also

### Date Range Constraints

var maxDate: Date?

The maximum date that the picker allows as input.

