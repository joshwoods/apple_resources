

- Foundation
- Date
- Date.IntervalFormatStyle
-  Date.IntervalFormatStyle.TimeStyle 

Type Alias

# Date.IntervalFormatStyle.TimeStyle

The type that defines time styles that vary in length or in their included components.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
typealias TimeStyle = Date.FormatStyle.TimeStyle
```

## Discussion

The exact format depends on the locale. Possible time styles include: omitted, shortened, standard, and complete.

The following code sample shows a variety of time style format results using the `en_US` locale.

```
if let today = Calendar.current.date(byAdding: .day, value: -120, to: Date()),
   let thirtyDaysBeforeToday = Calendar.current.date(byAdding: .day, value: -30, to: today) {
   // today: Apr 11, 2021 at 7:14 AM
   // thirtyDaysBeforeToday: Mar 12, 2021 at 7:14 AM

   // Create a Range.
   let last30days = thirtyDaysBeforeToday..

## See Also

### Supporting Types

typealias DateStyle

The type that defines date interval styles that vary in length or in their included components.

typealias Symbol

The type that supports customizing formatting templates using the date format style’s modifier functions, and constructing fixed-pattern date format strings.

