

- Core Foundation
-  CFCalendarGetIdentifier(\_:) 

Function

# CFCalendarGetIdentifier(\_:)

Returns the given calendar’s identifier.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCalendarGetIdentifier(_ calendar: CFCalendar!) -> CFCalendarIdentifier!
```

## Parameters 

`calendar`  

The calendar to examine.

## Return Value

A string representation of `calendar`’s identifier. Calendar identifier constants can be found in CFLocale. Ownership follows the The Get Rule.

