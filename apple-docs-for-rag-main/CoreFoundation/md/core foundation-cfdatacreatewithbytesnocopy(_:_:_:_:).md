

- Core Foundation
-  CFDataCreateWithBytesNoCopy(\_:\_:\_:\_:) 

Function

# CFDataCreateWithBytesNoCopy(\_:\_:\_:\_:)

Creates an immutable CFData object from an external (client-owned) byte buffer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDataCreateWithBytesNoCopy(
    _ allocator: CFAllocator!,
    _ bytes: UnsafePointer!,
    _ length: CFIndex,
    _ bytesDeallocator: CFAllocator!
) -> CFData!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`bytes`  

A pointer to the byte buffer to be used as the backing store of the CFData object.

`length`  

The number of bytes in the buffer `bytes`.

`bytesDeallocator`  

The allocator to use to deallocate the external buffer when the CFData object is deallocated. If the default allocator is suitable for this purpose, pass `NULL` or kCFAllocatorDefault. If you do not want the created CFData object to deallocate the buffer (that is, you assume responsibility for freeing it yourself), pass kCFAllocatorNull.

## Return Value

A new CFData object, or `NULL` if there was a problem creating the object. On a `NULL` return, the `bytes` buffer is left intact. Ownership follows the The Create Rule.

## Discussion

This function creates an immutable CFData object from a buffer of unstructured bytes. Unless the situation warrants otherwise, the created object does not copy the external buffer to internal storage but instead uses the buffer as its backing store. However, you should never count on the object using the external buffer since it could copy the buffer to internal storage or might even dump the buffer altogether and use alternative means for storing the bytes.

## See Also

### Creating a CFData Object

func CFDataCreate(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex) -> CFData!

Creates an immutable CFData object using data copied from a specified byte buffer.

func CFDataCreateCopy(CFAllocator!, CFData!) -> CFData!

Creates an immutable copy of a CFData object.

