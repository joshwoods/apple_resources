

- Core Foundation
-  CFReadStreamCreateWithFile(\_:\_:) 

Function

# CFReadStreamCreateWithFile(\_:\_:)

Creates a readable stream for a file.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFReadStreamCreateWithFile(
    _ alloc: CFAllocator!,
    _ fileURL: CFURL!
) -> CFReadStream!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`fileURL`  

The URL of the file to read. The URL must use the file scheme.

## Return Value

The new readable stream object, or `NULL` on failure. Ownership follows the The Create Rule.

## Discussion

You must open the stream, using CFReadStreamOpen(_:), before reading from it.

## See Also

### Creating a Read Stream

func CFReadStreamCreateWithBytesNoCopy(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex, CFAllocator!) -> CFReadStream!

Creates a readable stream for a block of memory.

