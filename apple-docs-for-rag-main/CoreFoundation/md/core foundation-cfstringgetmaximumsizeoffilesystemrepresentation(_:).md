

- Core Foundation
-  CFStringGetMaximumSizeOfFileSystemRepresentation(\_:) 

Function

# CFStringGetMaximumSizeOfFileSystemRepresentation(\_:)

Determines the upper bound on the number of bytes required to hold the file system representation of the string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringGetMaximumSizeOfFileSystemRepresentation(_ string: CFString!) -> CFIndex
```

## Parameters 

`string`  

The string to convert.

## Return Value

The upper bound on the number of bytes required to hold the file system representation of the string.

## Discussion

The result is returned quickly as a rough approximation, and could be much larger than the actual space required. The result includes space for the zero termination. If you are allocating a buffer for long-term storage, you should reallocate it to be the right size after calling CFStringGetFileSystemRepresentation(_:_:_:).

## See Also

### String File System Representations

func CFStringCreateWithFileSystemRepresentation(CFAllocator!, UnsafePointer&lt;CChar>!) -> CFString!

Creates a CFString from a zero-terminated POSIX file system representation.

func CFStringGetFileSystemRepresentation(CFString!, UnsafeMutablePointer&lt;CChar>!, CFIndex) -> Bool

Extracts the contents of a string as a `NULL`-terminated 8-bit string appropriate for passing to POSIX APIs.

