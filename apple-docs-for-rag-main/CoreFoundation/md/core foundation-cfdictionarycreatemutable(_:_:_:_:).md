

- Core Foundation
-  CFDictionaryCreateMutable(\_:\_:\_:\_:) 

Function

# CFDictionaryCreateMutable(\_:\_:\_:\_:)

Creates a new mutable dictionary.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDictionaryCreateMutable(
    _ allocator: CFAllocator!,
    _ capacity: CFIndex,
    _ keyCallBacks: UnsafePointer!,
    _ valueCallBacks: UnsafePointer!
) -> CFMutableDictionary!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new dictionary and its storage for key-value pairs. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`capacity`  

The maximum number of key-value pairs that can be contained by the new dictionary. The dictionary starts empty and can grow to this number of key-value pairs (and it can have less).

Pass `0` to specify that the maximum capacity is not limited. The value must not be negative.

`keyCallBacks`  

A pointer to a CFDictionaryKeyCallBacks structure initialized with the callbacks to use to retain, release, describe, and compare keys in the dictionary. A copy of the contents of the callbacks structure is made, so that a pointer to a structure on the stack can be passed in or can be reused for multiple collection creations.

This value may be `NULL`, which is treated as a valid structure of version `0` with all fields `NULL`. Otherwise, if any of the fields are not valid pointers to functions of the correct type, or this value is not a valid pointer to a `CFDictionaryKeyCallBacks` structure, the behavior is undefined. If any of the keys put into the collection is not one understood by one of the callback functions, the behavior when that callback function is used is undefined.

If the dictionary will contain only CFType objects, then pass a pointer to kCFTypeDictionaryKeyCallBacks as this parameter to use the default callback functions.

`valueCallBacks`  

A pointer to a CFDictionaryValueCallBacks structure initialized with the callbacks to use to retain, release, describe, and compare values in the dictionary. A copy of the contents of the callbacks structure is made, so that a pointer to a structure on the stack can be passed in or can be reused for multiple collection creations.

This value may be `NULL`, which is treated as a valid structure of version `0` with all fields `NULL`. Otherwise, if any of the fields are not valid pointers to functions of the correct type, or this value is not a valid pointer to a `CFDictionaryValueCallBacks` structure, the behavior is undefined. If any value put into the collection is not one understood by one of the callback functions, the behavior when that callback function is used is undefined.

If the dictionary will contain CFType objects only, then pass a pointer to kCFTypeDictionaryValueCallBacks as this parameter to use the default callback functions.

## Return Value

A new dictionary, or `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## See Also

### Creating a Mutable Dictionary

func CFDictionaryCreateMutableCopy(CFAllocator!, CFIndex, CFDictionary!) -> CFMutableDictionary!

Creates a new mutable dictionary with the key-value pairs from another dictionary.

