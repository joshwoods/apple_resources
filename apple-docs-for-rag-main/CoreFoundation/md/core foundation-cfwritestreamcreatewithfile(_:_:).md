

- Core Foundation
-  CFWriteStreamCreateWithFile(\_:\_:) 

Function

# CFWriteStreamCreateWithFile(\_:\_:)

Creates a writable stream for a file.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFWriteStreamCreateWithFile(
    _ alloc: CFAllocator!,
    _ fileURL: CFURL!
) -> CFWriteStream!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`fileURL`  

The URL of the file to which to write. The URL must use a file scheme.

## Return Value

The new write stream, or `NULL` on failure. Ownership follows the The Create Rule.

## Discussion

The stream overwrites an existing file unless you set the kCFStreamPropertyAppendToFile to kCFBooleanTrue with CFWriteStreamSetProperty(_:_:_:), in which case the stream appends data to the file.

You must open the stream, using CFWriteStreamOpen(_:), before writing to it.

## See Also

### Creating a Write Stream

func CFWriteStreamCreateWithAllocatedBuffers(CFAllocator!, CFAllocator!) -> CFWriteStream!

Creates a writable stream for a growable block of memory.

func CFWriteStreamCreateWithBuffer(CFAllocator!, UnsafeMutablePointer&lt;UInt8>!, CFIndex) -> CFWriteStream!

Creates a writable stream for a fixed-size block of memory.

