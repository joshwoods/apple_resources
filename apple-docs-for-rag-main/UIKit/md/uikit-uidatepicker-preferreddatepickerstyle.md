

- UIKit
- UIDatePicker
-  preferredDatePickerStyle 

Instance Property

# preferredDatePickerStyle

The preferred style of the date picker.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
@MainActor
var preferredDatePickerStyle: UIDatePickerStyle { get set }
```

## Discussion

Use this property to specify the display style that you prefer. If the style changes, the date picker may generate a layout pass to update the display.

The default style is UIDatePickerStyle.automatic. For a list of styles, see UIDatePickerStyle.

## See Also

### Configuring the date picker style

var datePickerStyle: UIDatePickerStyle

The current style of the date picker.

enum UIDatePickerStyle

Styles that determine the appearance of a date picker.

