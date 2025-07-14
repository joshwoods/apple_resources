

- Core Foundation
-  CFCalendarGetMinimumDaysInFirstWeek(\_:) 

Function

# CFCalendarGetMinimumDaysInFirstWeek(\_:)

Returns the minimum number of days in the first week of a specified calendar.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCalendarGetMinimumDaysInFirstWeek(_ calendar: CFCalendar!) -> CFIndex
```

## Parameters 

`calendar`  

The calendar to examine.

## Return Value

The minimum number of days in the first week of `calendar`.

## See Also

### Getting and Setting Day Information

func CFCalendarGetFirstWeekday(CFCalendar!) -> CFIndex

Returns the index of first weekday for a specified calendar.

func CFCalendarSetFirstWeekday(CFCalendar!, CFIndex)

Sets the first weekday for a calendar.

func CFCalendarSetMinimumDaysInFirstWeek(CFCalendar!, CFIndex)

Sets the minimum number of days in the first week of a specified calendar.

