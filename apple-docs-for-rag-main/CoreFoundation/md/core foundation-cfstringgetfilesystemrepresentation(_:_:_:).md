

- Core Foundation
-  CFStringGetFileSystemRepresentation(\_:\_:\_:) 

Function

# CFStringGetFileSystemRepresentation(\_:\_:\_:)

Extracts the contents of a string as a `NULL`-terminated 8-bit string appropriate for passing to POSIX APIs.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringGetFileSystemRepresentation(
    _ string: CFString!,
    _ buffer: UnsafeMutablePointer!,
    _ maxBufLen: CFIndex
) -> Bool
```

## Parameters 

`string`  

The string to convert.

`buffer`  

The C string buffer into which to copy the string. The buffer must be at least `maxBufLen` bytes in length. On return, the buffer contains the converted characters.

`maxBufLen`  

The maximum length of the buffer.

## Return Value

`true` if the string is correctly converted; `false` if the conversion fails, or the results don’t fit into the buffer.

## Discussion

You can use CFStringGetMaximumSizeOfFileSystemRepresentation(_:) if you want to make sure the buffer is of sufficient length.

## See Also

### String File System Representations

func CFStringCreateWithFileSystemRepresentation(CFAllocator!, UnsafePointer&lt;CChar>!) -> CFString!

Creates a CFString from a zero-terminated POSIX file system representation.

func CFStringGetMaximumSizeOfFileSystemRepresentation(CFString!) -> CFIndex

Determines the upper bound on the number of bytes required to hold the file system representation of the string.

