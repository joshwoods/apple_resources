

- AppKit
- NSDatePicker
-  maxDate 

Instance Property

# maxDate

The date picker’s maximum date value.

macOS

``` source
@MainActor
var maxDate: Date? { get set }
```

## Discussion

This property represents the maximum value that the date picker allows as input. `nil` indicates no maximum date.

## See Also

### Constraining the Displayable/Selectable Range

var minDate: Date?

The date picker’s minimum date value.

