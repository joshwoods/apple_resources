

- AppKit
- NSDatePickerCell
-  maxDate 

Instance Property

# maxDate

The maximum date that the picker allows as input.

macOS

``` source
@MainActor
var maxDate: Date? { get set }
```

## Discussion

Set this property to `nil` if you want to allow any value for the maximum date.

## See Also

### Date Range Constraints

var minDate: Date?

The minimum date that the picker allows as input.

