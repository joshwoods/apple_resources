

- Core Foundation
-  CFDataSetLength(\_:\_:) 

Function

# CFDataSetLength(\_:\_:)

Resets the length of a CFMutableData object’s internal byte buffer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDataSetLength(
    _ theData: CFMutableData!,
    _ length: CFIndex
)
```

## Parameters 

`theData`  

A CFMutableData object. If you pass an immutable CFData object, the behavior is not defined.

`length`  

The new size of `theData`’s byte buffer.

## Discussion

This function resets the length of a CFMutableData object’s underlying byte buffer to a new size. If that size is less than the current size, it truncates the excess bytes. If that size is greater than the current size, it zero-fills the extension to the byte buffer.

## See Also

### Modifying a Mutable Data Object

func CFDataAppendBytes(CFMutableData!, UnsafePointer&lt;UInt8>!, CFIndex)

Appends the bytes from a byte buffer to the contents of a CFData object.

func CFDataDeleteBytes(CFMutableData!, CFRange)

Deletes the bytes in a CFMutableData object within a specified range.

func CFDataReplaceBytes(CFMutableData!, CFRange, UnsafePointer&lt;UInt8>!, CFIndex)

Replaces those bytes in a CFMutableData object that fall within a specified range with other bytes.

func CFDataIncreaseLength(CFMutableData!, CFIndex)

Increases the length of a CFMutableData object’s internal byte buffer, zero-filling the extension to the buffer.

