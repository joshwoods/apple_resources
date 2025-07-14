

- Core Foundation
-  CFDateCompare(\_:\_:\_:) 

Function

# CFDateCompare(\_:\_:\_:)

Compares two `CFDate` objects and returns a comparison result.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDateCompare(
    _ theDate: CFDate!,
    _ otherDate: CFDate!,
    _ context: UnsafeMutableRawPointer!
) -> CFComparisonResult
```

## Parameters 

`theDate`  

The date to compare to `otherDate`.

`otherDate`  

The date to compare to `theDate`.

`context`  

Unused. Pass `NULL`.

## Return Value

A CFComparisonResult value that indicates whether `theDate` is equal to, less than, or greater than `otherDate`.

## See Also

### CFDate Miscellaneous Functions

func CFDateCreate(CFAllocator!, CFAbsoluteTime) -> CFDate!

Creates a `CFDate` object given an absolute time.

func CFDateGetAbsoluteTime(CFDate!) -> CFAbsoluteTime

Returns a `CFDate` object’s absolute time.

func CFDateGetTimeIntervalSinceDate(CFDate!, CFDate!) -> CFTimeInterval

Returns the number of elapsed seconds between the given `CFDate` objects.

func CFDateGetTypeID() -> CFTypeID

Returns the type identifier for the `CFDate` opaque type.

