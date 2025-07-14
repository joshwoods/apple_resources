

- Core Foundation
-  CFURLGetBytes(\_:\_:\_:) 

Function

# CFURLGetBytes(\_:\_:\_:)

Returns by reference the byte representation of a URL object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFURLGetBytes(
    _ url: CFURL!,
    _ buffer: UnsafeMutablePointer!,
    _ bufferLength: CFIndex
) -> CFIndex
```

## Parameters 

`url`  

The URL object to convert to a byte representation.

`buffer`  

The buffer where you want the bytes to be placed. If the buffer is of insufficient size, returns `-1` and no bytes are placed in buffer. If `NULL` the needed length is computed and returned. The returned bytes are the original bytes from which the URL was created (*not* including the base URL). If the URL was created from a string, the bytes are the bytes of the string encoded via UTF-8.

`bufferLength`  

The number of bytes in `buffer`.

## Return Value

Returns the number of bytes in `buffer` that were filled. If the buffer is of insufficient size, returns `-1`.

## See Also

### Getting URL Properties

func CFURLGetBaseURL(CFURL!) -> CFURL!

Returns the base URL of a given URL if it exists.

func CFURLGetByteRangeForComponent(CFURL!, CFURLComponentType, UnsafeMutablePointer&lt;CFRange>!) -> CFRange

Returns the range of the specified component in the bytes of a URL.

func CFURLGetTypeID() -> CFTypeID

Returns the type identifier for the `CFURL` opaque type.

func CFURLResourceIsReachable(CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Returns whether the resource pointed to by a file URL can be reached.

