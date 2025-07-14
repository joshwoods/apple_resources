

- Core Foundation
-  CFCalendarSetMinimumDaysInFirstWeek(\_:\_:) 

Function

# CFCalendarSetMinimumDaysInFirstWeek(\_:\_:)

Sets the minimum number of days in the first week of a specified calendar.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCalendarSetMinimumDaysInFirstWeek(
    _ calendar: CFCalendar!,
    _ mwd: CFIndex
)
```

## Parameters 

`calendar`  

The calendar to modify.

`mwd`  

The number to set as the minimum number of days in the first week of `calendar`.

## See Also

### Getting and Setting Day Information

func CFCalendarGetFirstWeekday(CFCalendar!) -> CFIndex

Returns the index of first weekday for a specified calendar.

func CFCalendarSetFirstWeekday(CFCalendar!, CFIndex)

Sets the first weekday for a calendar.

func CFCalendarGetMinimumDaysInFirstWeek(CFCalendar!) -> CFIndex

Returns the minimum number of days in the first week of a specified calendar.

