

- Core Foundation
-  CFDateGetTimeIntervalSinceDate(\_:\_:) 

Function

# CFDateGetTimeIntervalSinceDate(\_:\_:)

Returns the number of elapsed seconds between the given `CFDate` objects.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDateGetTimeIntervalSinceDate(
    _ theDate: CFDate!,
    _ otherDate: CFDate!
) -> CFTimeInterval
```

## Parameters 

`theDate`  

The date to compare to `otherDate`.

`otherDate`  

The date to compare to `theDate`.

## Return Value

The number of elapsed seconds between `theDate` and `otherDate`. The result is positive if `theDate` is later than `otherDate`.

## See Also

### CFDate Miscellaneous Functions

func CFDateCompare(CFDate!, CFDate!, UnsafeMutableRawPointer!) -> CFComparisonResult

Compares two `CFDate` objects and returns a comparison result.

func CFDateCreate(CFAllocator!, CFAbsoluteTime) -> CFDate!

Creates a `CFDate` object given an absolute time.

func CFDateGetAbsoluteTime(CFDate!) -> CFAbsoluteTime

Returns a `CFDate` object’s absolute time.

func CFDateGetTypeID() -> CFTypeID

Returns the type identifier for the `CFDate` opaque type.

