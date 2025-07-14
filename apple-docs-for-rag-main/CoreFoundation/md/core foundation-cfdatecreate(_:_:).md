

- Core Foundation
-  CFDateCreate(\_:\_:) 

Function

# CFDateCreate(\_:\_:)

Creates a `CFDate` object given an absolute time.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDateCreate(
    _ allocator: CFAllocator!,
    _ at: CFAbsoluteTime
) -> CFDate!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`at`  

The absolute time to convert to a CFDate object.

## Return Value

A date object that represents the absolute time `at`. The caller is responsible for releasing the `CFDate` object using CFRelease.

## Discussion

`CFDate` objects must always be created using absolute time. Time intervals are not supported.

## See Also

### CFDate Miscellaneous Functions

func CFDateCompare(CFDate!, CFDate!, UnsafeMutableRawPointer!) -> CFComparisonResult

Compares two `CFDate` objects and returns a comparison result.

func CFDateGetAbsoluteTime(CFDate!) -> CFAbsoluteTime

Returns a `CFDate` object’s absolute time.

func CFDateGetTimeIntervalSinceDate(CFDate!, CFDate!) -> CFTimeInterval

Returns the number of elapsed seconds between the given `CFDate` objects.

func CFDateGetTypeID() -> CFTypeID

Returns the type identifier for the `CFDate` opaque type.

