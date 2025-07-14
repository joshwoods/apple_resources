

- Core Foundation
-  CFCalendarGetMaximumRangeOfUnit(\_:\_:) 

Function

# CFCalendarGetMaximumRangeOfUnit(\_:\_:)

Returns the maximum range limits of the values that a specified unit can take on in a given calendar.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCalendarGetMaximumRangeOfUnit(
    _ calendar: CFCalendar!,
    _ unit: CFCalendarUnit
) -> CFRange
```

## Parameters 

`calendar`  

The calendar to examine.

`unit`  

A calendar unit. For valid values see CFCalendarUnit.

## Return Value

The maximum range limits of the values that the specified unit can take on in `calendar`. For example, in the Gregorian calendar the maximum ranges for the Day unit is 1-31.

## See Also

### Getting Ranges of Units

func CFCalendarGetRangeOfUnit(CFCalendar!, CFCalendarUnit, CFCalendarUnit, CFAbsoluteTime) -> CFRange

Returns the range of values that one unit can take on within a larger unit during which a specific absolute time occurs.

func CFCalendarGetOrdinalityOfUnit(CFCalendar!, CFCalendarUnit, CFCalendarUnit, CFAbsoluteTime) -> CFIndex

Returns the ordinal number of a calendrical unit within a larger unit at a specified absolute time.

func CFCalendarGetTimeRangeOfUnit(CFCalendar!, CFCalendarUnit, CFAbsoluteTime, UnsafeMutablePointer&lt;CFAbsoluteTime>!, UnsafeMutablePointer&lt;CFTimeInterval>!) -> Bool

Returns by reference the start time and duration of a given calendar unit that contains a given absolute time.

func CFCalendarGetMinimumRangeOfUnit(CFCalendar!, CFCalendarUnit) -> CFRange

Returns the minimum range limits of the values that a specified unit can take on in a given calendar.

