

- Core Foundation
-  CFCalendarCopyCurrent() 

Function

# CFCalendarCopyCurrent()

Returns a copy of the logical calendar for the current user.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCalendarCopyCurrent() -> CFCalendar!
```

## Return Value

The logical calendar for the current user that is formed from the settings for the current user’s chosen system locale overlaid with any custom settings the user has specified in System Preferences. This function may return a retained cached object, not a new object. Ownership follows the The Create Rule.

## Discussion

Settings you get from this calendar do not change if user defaults change so that your operations are consistent.

Typically you perform some operations on the returned object and then release it. The returned object may be cached, so you do not need to hold on to it indefinitely.

## See Also

### Creating a Calendar

func CFCalendarCreateWithIdentifier(CFAllocator!, CFCalendarIdentifier!) -> CFCalendar!

Returns a calendar object for the calendar identified by a calendar identifier.

