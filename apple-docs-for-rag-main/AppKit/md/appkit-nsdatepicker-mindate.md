

- AppKit
- NSDatePicker
-  minDate 

Instance Property

# minDate

The date picker’s minimum date value.

macOS

``` source
@MainActor
var minDate: Date? { get set }
```

## Discussion

This property represents the minimum value that the date picker allows as input. `nil` indicates no minimum date.

## See Also

### Constraining the Displayable/Selectable Range

var maxDate: Date?

The date picker’s maximum date value.

