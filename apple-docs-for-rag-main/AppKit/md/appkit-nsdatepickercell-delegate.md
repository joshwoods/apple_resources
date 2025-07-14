

- AppKit
- NSDatePickerCell
-  delegate 

Instance Property

# delegate

The delegate associated with the date picker.

macOS

``` source
@MainActor
weak var delegate: (any NSDatePickerCellDelegate)? { get set }
```

## Discussion

The delegate must conform to NSDatePickerCellDelegate.

