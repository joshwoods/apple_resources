

- Core Foundation
-  CFDictionaryCreate(\_:\_:\_:\_:\_:\_:) 

Function

# CFDictionaryCreate(\_:\_:\_:\_:\_:\_:)

Creates an immutable dictionary containing the specified key-value pairs.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDictionaryCreate(
    _ allocator: CFAllocator!,
    _ keys: UnsafeMutablePointer!,
    _ values: UnsafeMutablePointer!,
    _ numValues: CFIndex,
    _ keyCallBacks: UnsafePointer!,
    _ valueCallBacks: UnsafePointer!
) -> CFDictionary!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new dictionary. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`keys`  

A C array of the pointer-sized keys to be in the new dictionary. This value may be `NULL` if the `numValues` parameter is `0`. This C array is not changed or freed by this function. The value must be a valid pointer to a C array of at least `numValues` pointers.

`values`  

A C array of the pointer-sized values to be in the new dictionary. This value may be `NULL` if the `numValues` parameter is `0`. This C array is not changed or freed by this function. The value must be a valid pointer to a C array of at least `numValues` elements.

`numValues`  

The number of key-value pairs to copy from the `keys` and `values` C arrays into the new dictionary. This number will be the count of the dictionary; it must be non-negative and less than or equal to the actual number of keys or values.

`keyCallBacks`  

A pointer to a CFDictionaryKeyCallBacks structure initialized with the callbacks to use to retain, release, describe, and compare keys in the dictionary. A copy of the contents of the callbacks structure is made, so that a pointer to a structure on the stack can be passed in or can be reused for multiple collection creations.

This value may be `NULL`, which is treated as if a valid structure of version `0` with all fields `NULL` had been passed in. Otherwise, if any of the fields are not valid pointers to functions of the correct type, or this parameter is not a valid pointer to a CFDictionaryKeyCallBacks structure, the behavior is undefined. If any of the keys put into the collection is not one understood by one of the callback functions the behavior when that callback function is used is undefined.

If the collection will contain CFType objects only, then pass a pointer to kCFTypeDictionaryKeyCallBacks as this parameter to use the default callback functions.

`valueCallBacks`  

A pointer to a CFDictionaryValueCallBacks structure initialized with the callbacks to use to retain, release, describe, and compare values in the dictionary. A copy of the contents of the callbacks structure is made, so that a pointer to a structure on the stack can be passed in or can be reused for multiple collection creations.

This value may be `NULL`, which is treated as if a valid structure of version `0` with all fields `NULL` had been passed in. Otherwise, if any of the fields are not valid pointers to functions of the correct type, or this parameter is not a valid pointer to a CFDictionaryValueCallBacks structure, the behavior is undefined. If any value put into the collection is not one understood by one of the callback functions the behavior when that callback function is used is undefined.

If the collection will contain CFType objects only, then pass a pointer to kCFTypeDictionaryValueCallBacks as this parameter to use the default callback functions.

## Return Value

A new dictionary, or `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## See Also

### Creating a dictionary

func CFDictionaryCreateCopy(CFAllocator!, CFDictionary!) -> CFDictionary!

Creates and returns a new immutable dictionary with the key-value pairs of another dictionary.

