

- Core Foundation
-  CFWriteStreamCreateWithAllocatedBuffers(\_:\_:) 

Function

# CFWriteStreamCreateWithAllocatedBuffers(\_:\_:)

Creates a writable stream for a growable block of memory.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFWriteStreamCreateWithAllocatedBuffers(
    _ alloc: CFAllocator!,
    _ bufferAllocator: CFAllocator!
) -> CFWriteStream!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`bufferAllocator`  

The allocator to use to allocate memory for the stream’s memory buffers. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

## Return Value

A new write stream. Ownership follows the The Create Rule.

## Discussion

New buffers are allocated using `bufferAllocator` as bytes are written to the stream. At any point, you can recover the bytes thus far written by asking for the property kCFStreamPropertyDataWritten with CFWriteStreamCopyProperty(_:_:).

You must open the stream, using CFWriteStreamOpen(_:), before writing to it.

## See Also

### Creating a Write Stream

func CFWriteStreamCreateWithBuffer(CFAllocator!, UnsafeMutablePointer&lt;UInt8>!, CFIndex) -> CFWriteStream!

Creates a writable stream for a fixed-size block of memory.

func CFWriteStreamCreateWithFile(CFAllocator!, CFURL!) -> CFWriteStream!

Creates a writable stream for a file.

