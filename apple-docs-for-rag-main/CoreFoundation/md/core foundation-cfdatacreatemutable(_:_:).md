

- Core Foundation
-  CFDataCreateMutable(\_:\_:) 

Function

# CFDataCreateMutable(\_:\_:)

Creates an empty CFMutableData object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDataCreateMutable(
    _ allocator: CFAllocator!,
    _ capacity: CFIndex
) -> CFMutableData!
```

## Parameters 

`allocator`  

The CFAllocator object to be used to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`capacity`  

The maximum number of bytes that the CFData object can contain. The CFData object starts empty and can grow to contain this number of values (and it can have less).

Pass `0` to specify that the maximum capacity is not limited. The value must not be negative.

## Return Value

A CFMutableData object or `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## Discussion

This function creates an empty (that is, content-less) CFMutableData object. You can add raw data to this object with the CFDataAppendBytes(_:_:_:) function, and thereafter you can replace and delete characters with the appropriate CFMutableData functions. If the `capacity` parameter is greater than `0`, any attempt to add characters beyond this limit can result in undefined behavior.

## See Also

### Creating a Mutable Data Object

func CFDataCreateMutableCopy(CFAllocator!, CFIndex, CFData!) -> CFMutableData!

Creates a CFMutableData object by copying another CFData object.

