

- Core Foundation
-  CFURLGetByteRangeForComponent(\_:\_:\_:) 

Function

# CFURLGetByteRangeForComponent(\_:\_:\_:)

Returns the range of the specified component in the bytes of a URL.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFURLGetByteRangeForComponent(
    _ url: CFURL!,
    _ component: CFURLComponentType,
    _ rangeIncludingSeparators: UnsafeMutablePointer!
) -> CFRange
```

## Parameters 

`url`  

The URL containing `component`.

`component`  

The type of component in `anURL` whose range you want to obtain. See CFURLComponentType for possible values.

`rangeIncludingSeparators`  

Specifies the range of `component` including the sequences that separate component from the previous and next components. If there is no previous or next components, this function will match the range of the component itself. If `anURL` does not contain `component`, `rangeIncludingSeparators` is set to the location where the component would be inserted.

## Return Value

The range of bytes for `component` in the buffer returned by the CFURLGetBytes(_:_:_:) function. If `anURL` does not contain `component`, the first part of the returned range is set to kCFNotFound.

## Discussion

This function is intended to be used in conjunction with the CFURLGetBytes(_:_:_:) function, since the range returned is only applicable to the bytes returned by CFURLGetBytes(_:_:_:).

## See Also

### Getting URL Properties

func CFURLGetBaseURL(CFURL!) -> CFURL!

Returns the base URL of a given URL if it exists.

func CFURLGetBytes(CFURL!, UnsafeMutablePointer&lt;UInt8>!, CFIndex) -> CFIndex

Returns by reference the byte representation of a URL object.

func CFURLGetTypeID() -> CFTypeID

Returns the type identifier for the `CFURL` opaque type.

func CFURLResourceIsReachable(CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Returns whether the resource pointed to by a file URL can be reached.

