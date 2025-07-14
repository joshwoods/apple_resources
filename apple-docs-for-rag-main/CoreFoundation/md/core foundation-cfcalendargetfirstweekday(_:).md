

- Core Foundation
-  CFCalendarGetFirstWeekday(\_:) 

Function

# CFCalendarGetFirstWeekday(\_:)

Returns the index of first weekday for a specified calendar.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCalendarGetFirstWeekday(_ calendar: CFCalendar!) -> CFIndex
```

## Parameters 

`calendar`  

The calendar to examine.

## Return Value

The index of the first weekday of the specified calendar.

## See Also

### Getting and Setting Day Information

func CFCalendarSetFirstWeekday(CFCalendar!, CFIndex)

Sets the first weekday for a calendar.

func CFCalendarGetMinimumDaysInFirstWeek(CFCalendar!) -> CFIndex

Returns the minimum number of days in the first week of a specified calendar.

func CFCalendarSetMinimumDaysInFirstWeek(CFCalendar!, CFIndex)

Sets the minimum number of days in the first week of a specified calendar.

