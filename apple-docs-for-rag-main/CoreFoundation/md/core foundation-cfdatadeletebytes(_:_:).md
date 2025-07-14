

- Core Foundation
-  CFDataDeleteBytes(\_:\_:) 

Function

# CFDataDeleteBytes(\_:\_:)

Deletes the bytes in a CFMutableData object within a specified range.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDataDeleteBytes(
    _ theData: CFMutableData!,
    _ range: CFRange
)
```

## Parameters 

`theData`  

A CFMutableData object. If you pass an immutable CFData object, the behavior is not defined.

`range`  

The range of bytes (that is, the starting byte and the number of bytes from that point) to delete from `theData`’s byte buffer.

## See Also

### Modifying a Mutable Data Object

func CFDataAppendBytes(CFMutableData!, UnsafePointer&lt;UInt8>!, CFIndex)

Appends the bytes from a byte buffer to the contents of a CFData object.

func CFDataReplaceBytes(CFMutableData!, CFRange, UnsafePointer&lt;UInt8>!, CFIndex)

Replaces those bytes in a CFMutableData object that fall within a specified range with other bytes.

func CFDataIncreaseLength(CFMutableData!, CFIndex)

Increases the length of a CFMutableData object’s internal byte buffer, zero-filling the extension to the buffer.

func CFDataSetLength(CFMutableData!, CFIndex)

Resets the length of a CFMutableData object’s internal byte buffer.

