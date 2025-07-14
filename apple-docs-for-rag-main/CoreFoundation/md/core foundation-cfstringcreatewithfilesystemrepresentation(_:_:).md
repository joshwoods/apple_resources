

- Core Foundation
-  CFStringCreateWithFileSystemRepresentation(\_:\_:) 

Function

# CFStringCreateWithFileSystemRepresentation(\_:\_:)

Creates a CFString from a zero-terminated POSIX file system representation.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringCreateWithFileSystemRepresentation(
    _ alloc: CFAllocator!,
    _ buffer: UnsafePointer!
) -> CFString!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new string. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`buffer`  

The C string that you want to convert.

## Return Value

A string that represents `buffer`. The result is `NULL` if there was a problem in creating the string (possible if the conversion fails due to bytes in the buffer not being a valid sequence of bytes for the appropriate character encoding). Ownership follows the The Create Rule.

## See Also

### String File System Representations

func CFStringGetFileSystemRepresentation(CFString!, UnsafeMutablePointer&lt;CChar>!, CFIndex) -> Bool

Extracts the contents of a string as a `NULL`-terminated 8-bit string appropriate for passing to POSIX APIs.

func CFStringGetMaximumSizeOfFileSystemRepresentation(CFString!) -> CFIndex

Determines the upper bound on the number of bytes required to hold the file system representation of the string.

