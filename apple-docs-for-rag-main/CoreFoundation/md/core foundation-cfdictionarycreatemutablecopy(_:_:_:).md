

- Core Foundation
-  CFDictionaryCreateMutableCopy(\_:\_:\_:) 

Function

# CFDictionaryCreateMutableCopy(\_:\_:\_:)

Creates a new mutable dictionary with the key-value pairs from another dictionary.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDictionaryCreateMutableCopy(
    _ allocator: CFAllocator!,
    _ capacity: CFIndex,
    _ theDict: CFDictionary!
) -> CFMutableDictionary!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new dictionary and its storage for key-value pairs. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`capacity`  

The maximum number of key-value pairs that can be contained by the new dictionary. The dictionary starts with the same number of key-value pairs as `theDict` and can grow to this number of values (and it can have less).

Pass `0` to specify that the maximum capacity is not limited. If non-`0`, `capacity` must be greater than or equal to the count of `theDict`.

`theDict`  

The dictionary to copy. The keys and values from the dictionary are copied as pointers into the new dictionary, not that which the values point to (if anything). The keys and values are also retained by the new dictionary. The count of the new dictionary is the same as the count of `theDict`. The new dictionary uses the same callbacks as `theDict`.

## Return Value

A new dictionary that contains the same values as `theDict`. Ownership follows the The Create Rule.

## See Also

### Creating a Mutable Dictionary

func CFDictionaryCreateMutable(CFAllocator!, CFIndex, UnsafePointer&lt;CFDictionaryKeyCallBacks>!, UnsafePointer&lt;CFDictionaryValueCallBacks>!) -> CFMutableDictionary!

Creates a new mutable dictionary.

