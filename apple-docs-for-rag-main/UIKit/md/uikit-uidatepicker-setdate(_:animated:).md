

- UIKit
- UIDatePicker
-  setDate(\_:animated:) 

Instance Method

# setDate(\_:animated:)

Sets the date to display in the date picker, with an option to animate the setting.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setDate(
    _ date: Date,
    animated: Bool
)
```

## Parameters 

`date`  

An `NSDate` object representing the new date to display in the date picker.

`animated`  

true to animate the setting of the new date, otherwise false. The animation rotates the wheels until the new date and time is shown under the highlight rectangle.

## See Also

### Managing the date and calendar

var calendar: Calendar!

The calendar to use for the date picker.

var date: Date

The date displayed by the date picker.

var locale: Locale?

The locale used by the date picker.

var timeZone: TimeZone?

The time zone reflected in the date displayed by the date picker.

