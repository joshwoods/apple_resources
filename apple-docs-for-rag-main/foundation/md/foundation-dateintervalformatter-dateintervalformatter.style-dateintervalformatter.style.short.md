

- Foundation
- DateIntervalFormatter
- DateIntervalFormatter.Style
-  DateIntervalFormatter.Style.short 

Case

# DateIntervalFormatter.Style.short

An abbreviated date or time format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case short
```

## Discussion

For dates, this style displays the day, month, and year in numerical form using a format appropriate for the current locale. For example, formatting the date January 15, 2015 with this style results in the value “1/15/15” for US English and the value “15.1.15” for German.

For times, this style displays hours and minutes using a format appropriate for the current locale. For example, 12 hours and 33 minutes in the afternoon using a 12-hour clock results in the value “12:33 PM” for US English format and “12:33 nachm.” for German.

## See Also

### Constants

case none

No information for the date or time. Use this style when you do not want to include date or time information in the resulting string.

case medium

A medium length date or time format.

case long

A long length date or time format.

case full

A fully spelled out date or time format.

case none

No information for the date or time. Use this style when you do not want to include date or time information in the resulting string.

case medium

A medium length date or time format.

case long

A long length date or time format.

case full

A fully spelled out date or time format.

