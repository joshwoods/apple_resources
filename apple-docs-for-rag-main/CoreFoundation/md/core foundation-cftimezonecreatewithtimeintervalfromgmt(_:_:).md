

- Core Foundation
-  CFTimeZoneCreateWithTimeIntervalFromGMT(\_:\_:) 

Function

# CFTimeZoneCreateWithTimeIntervalFromGMT(\_:\_:)

Returns a time zone object for the specified time interval offset from Greenwich Mean Time (GMT).

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFTimeZoneCreateWithTimeIntervalFromGMT(
    _ allocator: CFAllocator!,
    _ ti: CFTimeInterval
) -> CFTimeZone!
```

## Parameters 

`allocator`  

The allocator object to use to allocate memory for the new time zone. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`ti`  

The offset, from GMT, of the new time zone.

## Return Value

A new time zone whose offset from GMT is given by the interval `ti`. The name of the new time zone is GMT +/- the offset, in hours and minutes. Time zones created with this function never have daylight savings, and the offset is constant no matter what the date. Ownership follows the The Create Rule.

## See Also

### Creating a Time Zone

func CFTimeZoneCreateWithName(CFAllocator!, CFString!, Bool) -> CFTimeZone!

Returns the time zone object identified by a given name or abbreviation.

func CFTimeZoneCreate(CFAllocator!, CFString!, CFData!) -> CFTimeZone!

Creates a time zone with a given name and data.

