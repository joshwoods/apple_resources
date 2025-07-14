

- UIKit
- UIDatePicker
-  datePickerStyle 

Instance Property

# datePickerStyle

The current style of the date picker.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
@MainActor
var datePickerStyle: UIDatePickerStyle { get }
```

## Discussion

This property always returns a concrete style, never UIDatePickerStyle.automatic.

## See Also

### Configuring the date picker style

var preferredDatePickerStyle: UIDatePickerStyle

The preferred style of the date picker.

enum UIDatePickerStyle

Styles that determine the appearance of a date picker.

