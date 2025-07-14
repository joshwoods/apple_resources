

- Core Foundation
-  CFCalendarCreateWithIdentifier(\_:\_:) 

Function

# CFCalendarCreateWithIdentifier(\_:\_:)

Returns a calendar object for the calendar identified by a calendar identifier.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCalendarCreateWithIdentifier(
    _ allocator: CFAllocator!,
    _ identifier: CFCalendarIdentifier!
) -> CFCalendar!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`identifier`  

A calendar identifier. Calendar identifier constants are given in CFLocale.

## Return Value

A calendar object for the calendar identified by `ident`. If the identifier is unknown (if, for example, it is either an unrecognized string, or the calendar is not supported by the current version of the operating system), returns `NULL`. Ownership follows the The Create Rule.

## See Also

### Creating a Calendar

func CFCalendarCopyCurrent() -> CFCalendar!

Returns a copy of the logical calendar for the current user.

