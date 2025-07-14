

- Core Foundation
-  CFDataIncreaseLength(\_:\_:) 

Function

# CFDataIncreaseLength(\_:\_:)

Increases the length of a CFMutableData object’s internal byte buffer, zero-filling the extension to the buffer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDataIncreaseLength(
    _ theData: CFMutableData!,
    _ extraLength: CFIndex
)
```

## Parameters 

`theData`  

A CFMutableData object. If you pass an immutable CFData object, the behavior is not defined.

`extraLength`  

The number of bytes by which to increase the byte buffer.

## Discussion

This function increases the length of a CFMutableData object’s underlying byte buffer to a new size, initializing the new bytes to `0`.

## See Also

### Modifying a Mutable Data Object

func CFDataAppendBytes(CFMutableData!, UnsafePointer&lt;UInt8>!, CFIndex)

Appends the bytes from a byte buffer to the contents of a CFData object.

func CFDataDeleteBytes(CFMutableData!, CFRange)

Deletes the bytes in a CFMutableData object within a specified range.

func CFDataReplaceBytes(CFMutableData!, CFRange, UnsafePointer&lt;UInt8>!, CFIndex)

Replaces those bytes in a CFMutableData object that fall within a specified range with other bytes.

func CFDataSetLength(CFMutableData!, CFIndex)

Resets the length of a CFMutableData object’s internal byte buffer.

