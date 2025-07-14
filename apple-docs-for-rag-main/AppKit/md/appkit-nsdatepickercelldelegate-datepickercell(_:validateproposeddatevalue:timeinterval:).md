

- AppKit
- NSDatePickerCellDelegate
-  datePickerCell(\_:validateProposedDateValue:timeInterval:) 

Instance Method

# datePickerCell(\_:validateProposedDateValue:timeInterval:)

The delegate receives this message each time the user attempts to change the receiver’s value, allowing the delegate the opportunity to override the change.

macOS

``` source
@MainActor
optional func datePickerCell(
    _ datePickerCell: NSDatePickerCell,
    validateProposedDateValue proposedDateValue: AutoreleasingUnsafeMutablePointer,
    timeInterval proposedTimeInterval: UnsafeMutablePointer?
)
```

## Parameters 

`datePickerCell`  

The cell that sent the message.

`proposedDateValue`  

On input, contains the proposed new date. The delegate may change this value before returning.

`proposedTimeInterval`  

On input, contains the proposed new time interval. The delegate may change this value before returning.

## Discussion

When returning a new `proposedDateValue`, the `NSDate` instance should be autoreleased, and the `proposedDateValue` should not be released by the delegate.

The `proposedDateValue` and `proposedTimeInterval` are guaranteed to lie between the dates returned by minDate and maxDate. If you modify these values, you should ensure that the new values are within the appropriate range.

