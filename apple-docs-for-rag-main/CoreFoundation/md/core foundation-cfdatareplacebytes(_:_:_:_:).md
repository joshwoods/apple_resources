

- Core Foundation
-  CFDataReplaceBytes(\_:\_:\_:\_:) 

Function

# CFDataReplaceBytes(\_:\_:\_:\_:)

Replaces those bytes in a CFMutableData object that fall within a specified range with other bytes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDataReplaceBytes(
    _ theData: CFMutableData!,
    _ range: CFRange,
    _ newBytes: UnsafePointer!,
    _ newLength: CFIndex
)
```

## Parameters 

`theData`  

A CFMutableData object. If you pass an immutable CFData object, the behavior is not defined.

`range`  

The range of bytes (that is, the starting byte and the number of bytes from that point) to delete from `theData`’s byte buffer.

`newBytes`  

A pointer to the buffer containing the replacement bytes.

`newLength`  

The number of bytes in the byte buffer `newBytes`.

## See Also

### Modifying a Mutable Data Object

func CFDataAppendBytes(CFMutableData!, UnsafePointer&lt;UInt8>!, CFIndex)

Appends the bytes from a byte buffer to the contents of a CFData object.

func CFDataDeleteBytes(CFMutableData!, CFRange)

Deletes the bytes in a CFMutableData object within a specified range.

func CFDataIncreaseLength(CFMutableData!, CFIndex)

Increases the length of a CFMutableData object’s internal byte buffer, zero-filling the extension to the buffer.

func CFDataSetLength(CFMutableData!, CFIndex)

Resets the length of a CFMutableData object’s internal byte buffer.

