

- Foundation
- DateIntervalFormatter
- DateIntervalFormatter.Style
-  DateIntervalFormatter.Style.medium 

Case

# DateIntervalFormatter.Style.medium

A medium length date or time format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case medium
```

## Discussion

For dates, this style displays the numerical day and year and an abbreviated spelling of the month using a format appropriate for the current locale. For example, formatting the date January 15, 2015 with this style results in the value “Jan 15, 2015” for US English and the value “15. Jan. 2015” for German.

For times, this style displays hours, minutes, and seconds using a format appropriate for the current locale. For example, 12 hours, 33 minutes, and 29 seconds in the afternoon using a 12-hour clock results in the value “12:33:29 PM” for US English 12-hour format and “12:33:29 nachm.” for German.

## See Also

### Constants

case none

No information for the date or time. Use this style when you do not want to include date or time information in the resulting string.

case short

An abbreviated date or time format.

case long

A long length date or time format.

case full

A fully spelled out date or time format.

case none

No information for the date or time. Use this style when you do not want to include date or time information in the resulting string.

case short

An abbreviated date or time format.

case long

A long length date or time format.

case full

A fully spelled out date or time format.

