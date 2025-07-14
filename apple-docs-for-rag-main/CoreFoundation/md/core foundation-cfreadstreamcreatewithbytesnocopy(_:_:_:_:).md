

- Core Foundation
-  CFReadStreamCreateWithBytesNoCopy(\_:\_:\_:\_:) 

Function

# CFReadStreamCreateWithBytesNoCopy(\_:\_:\_:\_:)

Creates a readable stream for a block of memory.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFReadStreamCreateWithBytesNoCopy(
    _ alloc: CFAllocator!,
    _ bytes: UnsafePointer!,
    _ length: CFIndex,
    _ bytesDeallocator: CFAllocator!
) -> CFReadStream!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`bytes`  

The memory buffer to read. This memory must exist for the lifetime of the new stream.

`length`  

The size of `bytes`.

`bytesDeallocator`  

The allocator to use to deallocate `bytes` when the stream is deallocated. Pass kCFAllocatorNull to prevent the stream from deallocating `bytes`.

## Return Value

The new read stream, or `NULL` on failure. Ownership follows the The Create Rule.

## Discussion

You must open the stream, using CFReadStreamOpen(_:), before reading from it.

## See Also

### Creating a Read Stream

func CFReadStreamCreateWithFile(CFAllocator!, CFURL!) -> CFReadStream!

Creates a readable stream for a file.

