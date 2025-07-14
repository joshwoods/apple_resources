

- Core Foundation
-  CFDateGetAbsoluteTime(\_:) 

Function

# CFDateGetAbsoluteTime(\_:)

Returns a `CFDate` object’s absolute time.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDateGetAbsoluteTime(_ theDate: CFDate!) -> CFAbsoluteTime
```

## Parameters 

`theDate`  

The date to examine.

## Return Value

The absolute time of `theDate`.

## Discussion

Absolute time is measured in seconds relative to the absolute reference date of Jan 1 2001 00:00:00 GMT. A positive value represents a date after the reference date, a negative value represents a date before it. For example, the absolute time -32940326 is equivalent to December 16th, 1999 at 17:54:34.

## See Also

### CFDate Miscellaneous Functions

func CFDateCompare(CFDate!, CFDate!, UnsafeMutableRawPointer!) -> CFComparisonResult

Compares two `CFDate` objects and returns a comparison result.

func CFDateCreate(CFAllocator!, CFAbsoluteTime) -> CFDate!

Creates a `CFDate` object given an absolute time.

func CFDateGetTimeIntervalSinceDate(CFDate!, CFDate!) -> CFTimeInterval

Returns the number of elapsed seconds between the given `CFDate` objects.

func CFDateGetTypeID() -> CFTypeID

Returns the type identifier for the `CFDate` opaque type.

