

- Core Foundation
-  CFDataGetLength(\_:) 

Function

# CFDataGetLength(\_:)

Returns the number of bytes contained by a CFData object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDataGetLength(_ theData: CFData!) -> CFIndex
```

## Parameters 

`theData`  

The CFData object to examine.

## Return Value

An index that specifies the number of bytes in `theData`.

## See Also

### Examining a CFData Object

func CFDataGetBytePtr(CFData!) -> UnsafePointer&lt;UInt8>!

Returns a read-only pointer to the bytes of a CFData object.

func CFDataGetBytes(CFData!, CFRange, UnsafeMutablePointer&lt;UInt8>!)

Copies the byte contents of a CFData object to an external buffer.

func CFDataFind(CFData!, CFData!, CFRange, CFDataSearchFlags) -> CFRange

Finds and returns the range within a data object of the first occurrence of the given data, within a given range, subject to any given options.

