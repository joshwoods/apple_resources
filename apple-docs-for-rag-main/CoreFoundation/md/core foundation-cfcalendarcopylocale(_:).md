

- Core Foundation
-  CFCalendarCopyLocale(\_:) 

Function

# CFCalendarCopyLocale(\_:)

Returns a locale object for a specified calendar.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCalendarCopyLocale(_ calendar: CFCalendar!) -> CFLocale!
```

## Parameters 

`calendar`  

The calendar to examine.

## Return Value

A copy of the locale object for the specified calendar. Ownership follows the The Create Rule.

## See Also

### Getting and Setting the Locale

func CFCalendarSetLocale(CFCalendar!, CFLocale!)

Sets the locale for a calendar.

