

- Core Foundation
-  CFDataCreate(\_:\_:\_:) 

Function

# CFDataCreate(\_:\_:\_:)

Creates an immutable CFData object using data copied from a specified byte buffer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDataCreate(
    _ allocator: CFAllocator!,
    _ bytes: UnsafePointer!,
    _ length: CFIndex
) -> CFData!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`bytes`  

A pointer to the byte buffer that contains the raw data to be copied into `theData`.

`length`  

The number of bytes in the buffer (`bytes`).

## Return Value

A new CFData object, or `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## Discussion

You must supply a count of the bytes in the buffer. This function always copies the bytes in the provided buffer into internal storage.

## See Also

### Creating a CFData Object

func CFDataCreateCopy(CFAllocator!, CFData!) -> CFData!

Creates an immutable copy of a CFData object.

func CFDataCreateWithBytesNoCopy(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex, CFAllocator!) -> CFData!

Creates an immutable CFData object from an external (client-owned) byte buffer.

