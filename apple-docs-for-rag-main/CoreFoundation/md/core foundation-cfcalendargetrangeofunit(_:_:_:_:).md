

- Core Foundation
-  CFCalendarGetRangeOfUnit(\_:\_:\_:\_:) 

Function

# CFCalendarGetRangeOfUnit(\_:\_:\_:\_:)

Returns the range of values that one unit can take on within a larger unit during which a specific absolute time occurs.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCalendarGetRangeOfUnit(
    _ calendar: CFCalendar!,
    _ smallerUnit: CFCalendarUnit,
    _ biggerUnit: CFCalendarUnit,
    _ at: CFAbsoluteTime
) -> CFRange
```

## Parameters 

`calendar`  

The calendar to examine.

`smallerUnit`  

A calendar unit. For valid values see CFCalendarUnit.

`biggerUnit`  

A calendar unit. For valid values see CFCalendarUnit.

`at`  

An absolute time.

## Return Value

The range of values that the calendar unit specified by `smallerUnit` can take on within the calendar unit specified by `biggerUnit` that includes the absolute time `at`. For example, the range the Day unit can take on in the Month in which the absolute time lies.

## Discussion

If `biggerUnit` is not logically bigger than `smallerUnit` in the calendar, or the given combination of units does not make sense (or is a computation which is undefined), the result is `{kCFNotFound, kCFNotFound`}.

## See Also

### Getting Ranges of Units

func CFCalendarGetOrdinalityOfUnit(CFCalendar!, CFCalendarUnit, CFCalendarUnit, CFAbsoluteTime) -> CFIndex

Returns the ordinal number of a calendrical unit within a larger unit at a specified absolute time.

func CFCalendarGetTimeRangeOfUnit(CFCalendar!, CFCalendarUnit, CFAbsoluteTime, UnsafeMutablePointer&lt;CFAbsoluteTime>!, UnsafeMutablePointer&lt;CFTimeInterval>!) -> Bool

Returns by reference the start time and duration of a given calendar unit that contains a given absolute time.

func CFCalendarGetMaximumRangeOfUnit(CFCalendar!, CFCalendarUnit) -> CFRange

Returns the maximum range limits of the values that a specified unit can take on in a given calendar.

func CFCalendarGetMinimumRangeOfUnit(CFCalendar!, CFCalendarUnit) -> CFRange

Returns the minimum range limits of the values that a specified unit can take on in a given calendar.

