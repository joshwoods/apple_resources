

- Core Foundation
-  CFCalendarSetFirstWeekday(\_:\_:) 

Function

# CFCalendarSetFirstWeekday(\_:\_:)

Sets the first weekday for a calendar.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCalendarSetFirstWeekday(
    _ calendar: CFCalendar!,
    _ wkdy: CFIndex
)
```

## Parameters 

`calendar`  

The calendar to modify.

`wkdy`  

The index to set for the first weekday of `calendar`.

## See Also

### Getting and Setting Day Information

func CFCalendarGetFirstWeekday(CFCalendar!) -> CFIndex

Returns the index of first weekday for a specified calendar.

func CFCalendarGetMinimumDaysInFirstWeek(CFCalendar!) -> CFIndex

Returns the minimum number of days in the first week of a specified calendar.

func CFCalendarSetMinimumDaysInFirstWeek(CFCalendar!, CFIndex)

Sets the minimum number of days in the first week of a specified calendar.

