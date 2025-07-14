

- Core Foundation
-  CFDataGetBytePtr(\_:) 

Function

# CFDataGetBytePtr(\_:)

Returns a read-only pointer to the bytes of a CFData object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDataGetBytePtr(_ theData: CFData!) -> UnsafePointer!
```

## Parameters 

`theData`  

The CFData object to examine.

## Return Value

A read-only pointer to the bytes associated with `theData`.

## Discussion

This function is guaranteed to return a pointer to a CFData object’s internal bytes. CFData, unlike CFString, does not hide its internal storage.

## See Also

### Examining a CFData Object

func CFDataGetBytes(CFData!, CFRange, UnsafeMutablePointer&lt;UInt8>!)

Copies the byte contents of a CFData object to an external buffer.

func CFDataGetLength(CFData!) -> CFIndex

Returns the number of bytes contained by a CFData object.

func CFDataFind(CFData!, CFData!, CFRange, CFDataSearchFlags) -> CFRange

Finds and returns the range within a data object of the first occurrence of the given data, within a given range, subject to any given options.

