

- Core Foundation
-  CFCalendarSetLocale(\_:\_:) 

Function

# CFCalendarSetLocale(\_:\_:)

Sets the locale for a calendar.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCalendarSetLocale(
    _ calendar: CFCalendar!,
    _ locale: CFLocale!
)
```

## Parameters 

`calendar`  

The calendar to modify.

`locale`  

The locale to set for `calendar`.

## See Also

### Getting and Setting the Locale

func CFCalendarCopyLocale(CFCalendar!) -> CFLocale!

Returns a locale object for a specified calendar.

