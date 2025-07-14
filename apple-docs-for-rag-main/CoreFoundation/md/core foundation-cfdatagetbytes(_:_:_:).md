

- Core Foundation
-  CFDataGetBytes(\_:\_:\_:) 

Function

# CFDataGetBytes(\_:\_:\_:)

Copies the byte contents of a CFData object to an external buffer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDataGetBytes(
    _ theData: CFData!,
    _ range: CFRange,
    _ buffer: UnsafeMutablePointer!
)
```

## Parameters 

`theData`  

The CFData object to examine.

`range`  

The range of bytes in `theData` to get. To get all of the contents, pass `CFRangeMake(0,CFDataGetLength(theData))`.

`buffer`  

A pointer to the byte buffer of length `range.length` that is allocated on the stack or heap. On return, the buffer contains the requested range of bytes.

## See Also

### Examining a CFData Object

func CFDataGetBytePtr(CFData!) -> UnsafePointer&lt;UInt8>!

Returns a read-only pointer to the bytes of a CFData object.

func CFDataGetLength(CFData!) -> CFIndex

Returns the number of bytes contained by a CFData object.

func CFDataFind(CFData!, CFData!, CFRange, CFDataSearchFlags) -> CFRange

Finds and returns the range within a data object of the first occurrence of the given data, within a given range, subject to any given options.

