

- Core Foundation
-  CFDataFind(\_:\_:\_:\_:) 

Function

# CFDataFind(\_:\_:\_:\_:)

Finds and returns the range within a data object of the first occurrence of the given data, within a given range, subject to any given options.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFDataFind(
    _ theData: CFData!,
    _ dataToFind: CFData!,
    _ searchRange: CFRange,
    _ compareOptions: CFDataSearchFlags
) -> CFRange
```

## Parameters 

`theData`  

The data object within which to search.

`dataToFind`  

The data to find. Must not be `NULL`.

`searchRange`  

The range within `theData` to be searched.

`compareOptions`  

A bit mask specifying search options. The CFDataSearchFlags options can be specified singly or combined with the C bitwise `OR` operator

## Return Value

The range representing the location and length of `dataToFind` within `searchRange`, modulo the options in `compareOptions`. The range returned is relative to the start of the searched data, not the passed-in search range. Returns kCFNotFound if `dataToFind` is not found.

## See Also

### Examining a CFData Object

func CFDataGetBytePtr(CFData!) -> UnsafePointer&lt;UInt8>!

Returns a read-only pointer to the bytes of a CFData object.

func CFDataGetBytes(CFData!, CFRange, UnsafeMutablePointer&lt;UInt8>!)

Copies the byte contents of a CFData object to an external buffer.

func CFDataGetLength(CFData!) -> CFIndex

Returns the number of bytes contained by a CFData object.

