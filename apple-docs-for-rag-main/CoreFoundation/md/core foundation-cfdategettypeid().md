

- Core Foundation
-  CFDateGetTypeID() 

Function

# CFDateGetTypeID()

Returns the type identifier for the `CFDate` opaque type.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDateGetTypeID() -> CFTypeID
```

## Return Value

The type identifier for the CFDate opaque type.

## See Also

### CFDate Miscellaneous Functions

func CFDateCompare(CFDate!, CFDate!, UnsafeMutableRawPointer!) -> CFComparisonResult

Compares two `CFDate` objects and returns a comparison result.

func CFDateCreate(CFAllocator!, CFAbsoluteTime) -> CFDate!

Creates a `CFDate` object given an absolute time.

func CFDateGetAbsoluteTime(CFDate!) -> CFAbsoluteTime

Returns a `CFDate` object’s absolute time.

func CFDateGetTimeIntervalSinceDate(CFDate!, CFDate!) -> CFTimeInterval

Returns the number of elapsed seconds between the given `CFDate` objects.

