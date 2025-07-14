

- Core Foundation
-  CFTimeZoneCreate(\_:\_:\_:) 

Function

# CFTimeZoneCreate(\_:\_:\_:)

Creates a time zone with a given name and data.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFTimeZoneCreate(
    _ allocator: CFAllocator!,
    _ name: CFString!,
    _ data: CFData!
) -> CFTimeZone!
```

## Parameters 

`allocator`  

The allocator object to use to allocate memory for the new time zone. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`name`  

The name of the time zone to create.

`data`  

The data to use to initialize the time zone. The contents of the data should be the same as that found within the time-zone files located at `/usr/share/zoneinfo`.

## Return Value

A time zone corresponding to `name` and `data`. Ownership follows the The Create Rule.

## Discussion

You typically do not call this function directly. Use the CFTimeZoneCreateWithName(_:_:_:) function to obtain a time zone given its name.

## See Also

### Creating a Time Zone

func CFTimeZoneCreateWithName(CFAllocator!, CFString!, Bool) -> CFTimeZone!

Returns the time zone object identified by a given name or abbreviation.

func CFTimeZoneCreateWithTimeIntervalFromGMT(CFAllocator!, CFTimeInterval) -> CFTimeZone!

Returns a time zone object for the specified time interval offset from Greenwich Mean Time (GMT).

