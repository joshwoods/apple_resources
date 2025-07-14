

- Core Foundation
-  CFURLGetTypeID() 

Function

# CFURLGetTypeID()

Returns the type identifier for the `CFURL` opaque type.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFURLGetTypeID() -> CFTypeID
```

## Return Value

The type identifier for the `CFURL` opaque type.

## See Also

### Getting URL Properties

func CFURLGetBaseURL(CFURL!) -> CFURL!

Returns the base URL of a given URL if it exists.

func CFURLGetBytes(CFURL!, UnsafeMutablePointer&lt;UInt8>!, CFIndex) -> CFIndex

Returns by reference the byte representation of a URL object.

func CFURLGetByteRangeForComponent(CFURL!, CFURLComponentType, UnsafeMutablePointer&lt;CFRange>!) -> CFRange

Returns the range of the specified component in the bytes of a URL.

func CFURLResourceIsReachable(CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Returns whether the resource pointed to by a file URL can be reached.

