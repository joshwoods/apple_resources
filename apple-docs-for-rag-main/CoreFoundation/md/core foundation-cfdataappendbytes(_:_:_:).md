

- Core Foundation
-  CFDataAppendBytes(\_:\_:\_:) 

Function

# CFDataAppendBytes(\_:\_:\_:)

Appends the bytes from a byte buffer to the contents of a CFData object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDataAppendBytes(
    _ theData: CFMutableData!,
    _ bytes: UnsafePointer!,
    _ length: CFIndex
)
```

## Parameters 

`theData`  

A CFMutableData object. If you pass an immutable CFData object, the behavior is not defined.

`bytes`  

A pointer to the buffer of bytes to be added to `theData`.

`length`  

The number of bytes in the byte buffer `bytes`.

## See Also

### Modifying a Mutable Data Object

func CFDataDeleteBytes(CFMutableData!, CFRange)

Deletes the bytes in a CFMutableData object within a specified range.

func CFDataReplaceBytes(CFMutableData!, CFRange, UnsafePointer&lt;UInt8>!, CFIndex)

Replaces those bytes in a CFMutableData object that fall within a specified range with other bytes.

func CFDataIncreaseLength(CFMutableData!, CFIndex)

Increases the length of a CFMutableData object’s internal byte buffer, zero-filling the extension to the buffer.

func CFDataSetLength(CFMutableData!, CFIndex)

Resets the length of a CFMutableData object’s internal byte buffer.

