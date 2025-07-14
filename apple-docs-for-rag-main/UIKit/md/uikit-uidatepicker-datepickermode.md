

- UIKit
- UIDatePicker
-  datePickerMode 

Instance Property

# datePickerMode

The mode of the date picker.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var datePickerMode: UIDatePicker.Mode { get set }
```

## Discussion

Use this property to change the type of information displayed by the date picker. It determines whether the date picker allows selection of a date, a time, both date and time, or a countdown time. The default mode is UIDatePicker.Mode.dateAndTime. See UIDatePicker.Mode for a list of mode constants.

## See Also

### Configuring the date picker mode

enum Mode

The mode displayed by the date picker.

