

- Core Foundation
-  CFDataCreateCopy(\_:\_:) 

Function

# CFDataCreateCopy(\_:\_:)

Creates an immutable copy of a CFData object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDataCreateCopy(
    _ allocator: CFAllocator!,
    _ theData: CFData!
) -> CFData!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`theData`  

The CFData object to copy.

## Return Value

An immutable copy of `theData`, or `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## Discussion

The resulting object has the same byte contents as the original object, but it is always immutable. If the specified allocator and the allocator of the original object are the same, and the string is already immutable, this function may simply increment the retain count without making a true copy. To the caller, however, the resulting object is a true immutable copy, except the operation was more efficient.

Use this function when you need to pass a CFData object into another function by value (not reference).

## See Also

### Creating a CFData Object

func CFDataCreate(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex) -> CFData!

Creates an immutable CFData object using data copied from a specified byte buffer.

func CFDataCreateWithBytesNoCopy(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex, CFAllocator!) -> CFData!

Creates an immutable CFData object from an external (client-owned) byte buffer.

