

- Core Foundation
-  CFURLGetBaseURL(\_:) 

Function

# CFURLGetBaseURL(\_:)

Returns the base URL of a given URL if it exists.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFURLGetBaseURL(_ anURL: CFURL!) -> CFURL!
```

## Parameters 

`anURL`  

The `CFURL` object to examine.

## Return Value

A `CFURL` object representing the base URL of `anURL`. Ownership follows the get rule. See The Get Rule.

## See Also

### Getting URL Properties

func CFURLGetBytes(CFURL!, UnsafeMutablePointer&lt;UInt8>!, CFIndex) -> CFIndex

Returns by reference the byte representation of a URL object.

func CFURLGetByteRangeForComponent(CFURL!, CFURLComponentType, UnsafeMutablePointer&lt;CFRange>!) -> CFRange

Returns the range of the specified component in the bytes of a URL.

func CFURLGetTypeID() -> CFTypeID

Returns the type identifier for the `CFURL` opaque type.

func CFURLResourceIsReachable(CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Returns whether the resource pointed to by a file URL can be reached.

