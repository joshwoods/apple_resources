

- Core Foundation
-  CFCalendarCopyTimeZone(\_:) 

Function

# CFCalendarCopyTimeZone(\_:)

Returns a time zone object for a specified calendar.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCalendarCopyTimeZone(_ calendar: CFCalendar!) -> CFTimeZone!
```

## Parameters 

`calendar`  

The calendar to examine.

## Return Value

A copy of the time zone object for the specified calendar. Ownership follows the The Create Rule.

## See Also

### Getting and Setting the Time Zone

func CFCalendarSetTimeZone(CFCalendar!, CFTimeZone!)

Sets the time zone for a calendar.

