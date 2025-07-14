

- Core Foundation
-  CFDataCreateMutableCopy(\_:\_:\_:) 

Function

# CFDataCreateMutableCopy(\_:\_:\_:)

Creates a CFMutableData object by copying another CFData object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDataCreateMutableCopy(
    _ allocator: CFAllocator!,
    _ capacity: CFIndex,
    _ theData: CFData!
) -> CFMutableData!
```

## Parameters 

`allocator`  

The CFAllocator object to be used to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`capacity`  

The maximum number of bytes that the CFData object can contain. The CFData object starts with the same length as the original object, and can grow to contain this number of bytes.

Pass `0` to specify that the maximum capacity is not limited. If non-`0`, `capacity` must be greater than or equal to the length of `theData`.

`theData`  

The CFData object to be copied.

## Return Value

A CFMutableData object that has the same contents as the original object. Returns `NULL` if there was a problem copying the object. Ownership follows the The Create Rule.

## See Also

### Creating a Mutable Data Object

func CFDataCreateMutable(CFAllocator!, CFIndex) -> CFMutableData!

Creates an empty CFMutableData object.

