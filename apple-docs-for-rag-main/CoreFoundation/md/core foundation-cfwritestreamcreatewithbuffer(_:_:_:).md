

- Core Foundation
-  CFWriteStreamCreateWithBuffer(\_:\_:\_:) 

Function

# CFWriteStreamCreateWithBuffer(\_:\_:\_:)

Creates a writable stream for a fixed-size block of memory.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFWriteStreamCreateWithBuffer(
    _ alloc: CFAllocator!,
    _ buffer: UnsafeMutablePointer!,
    _ bufferCapacity: CFIndex
) -> CFWriteStream!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`buffer`  

The memory buffer into which to write data. This buffer must exist for the lifetime of the stream.

`bufferCapacity`  

The size of `buffer` and the maximum number of bytes that can be written.

## Return Value

A new write stream, or `NULL` on failure. Ownership follows the The Create Rule.

## Discussion

When `buffer` is filled after writing `bufferCapacity` bytes, the stream is exhausted and its status becomes CFStreamStatus.atEnd.

You must open the stream, using CFWriteStreamOpen(_:), before writing to it.

## See Also

### Creating a Write Stream

func CFWriteStreamCreateWithAllocatedBuffers(CFAllocator!, CFAllocator!) -> CFWriteStream!

Creates a writable stream for a growable block of memory.

func CFWriteStreamCreateWithFile(CFAllocator!, CFURL!) -> CFWriteStream!

Creates a writable stream for a file.

