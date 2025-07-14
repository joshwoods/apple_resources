

- Core Foundation
-  CFCalendarSetTimeZone(\_:\_:) 

Function

# CFCalendarSetTimeZone(\_:\_:)

Sets the time zone for a calendar.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCalendarSetTimeZone(
    _ calendar: CFCalendar!,
    _ tz: CFTimeZone!
)
```

## Parameters 

`calendar`  

The calendar to modify.

`tz`  

The time zone to set for `calendar`.

## See Also

### Getting and Setting the Time Zone

func CFCalendarCopyTimeZone(CFCalendar!) -> CFTimeZone!

Returns a time zone object for a specified calendar.

