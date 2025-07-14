

- UIKit
- UIDatePicker
-  date 

Instance Property

# date

The date displayed by the date picker.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var date: Date { get set }
```

## Discussion

Use this property to get and set the currently selected date. The default value of this property is the date when the UIDatePicker object is created. Setting this property animates the date picker by spinning the wheels to the new date and time; if you don’t want any animation to occur when you set the date, use the setDate(_:animated:) method, passing false for the `animated` parameter. This behavior of this property is undefined when the mode is set to UIDatePicker.Mode.countDownTimer; refer instead to the countDownDuration property.

## See Also

### Managing the date and calendar

var calendar: Calendar!

The calendar to use for the date picker.

var locale: Locale?

The locale used by the date picker.

func setDate(Date, animated: Bool)

Sets the date to display in the date picker, with an option to animate the setting.

var timeZone: TimeZone?

The time zone reflected in the date displayed by the date picker.

