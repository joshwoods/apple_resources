

- AppKit
-  NSDatePickerCellDelegate 

Protocol

# NSDatePickerCellDelegate

A set of optional methods implemented by delegates of NSDatePickerCell objects.

macOS

``` source
protocol NSDatePickerCellDelegate : NSObjectProtocol
```

## Topics

### Content Validation

func datePickerCell(NSDatePickerCell, validateProposedDateValue: AutoreleasingUnsafeMutablePointer&lt;NSDate>, timeInterval: UnsafeMutablePointer&lt;TimeInterval>?)

The delegate receives this message each time the user attempts to change the receiver’s value, allowing the delegate the opportunity to override the change.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Cells

class NSDatePickerCell

An object that controls the behavior of a date picker, or of a single date picker cell in a matrix.

