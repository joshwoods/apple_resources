

- Core Foundation
-  CFDictionaryCreateCopy(\_:\_:) 

Function

# CFDictionaryCreateCopy(\_:\_:)

Creates and returns a new immutable dictionary with the key-value pairs of another dictionary.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDictionaryCreateCopy(
    _ allocator: CFAllocator!,
    _ theDict: CFDictionary!
) -> CFDictionary!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new dictionary. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`theDict`  

The dictionary to copy. The keys and values from the dictionary are copied as pointers into the new dictionary. However, the keys and values are also retained by the new dictionary. The count of the new dictionary is the same as the count of `theDict`. The new dictionary uses the same callbacks as `theDict`.

## Return Value

A new dictionary that contains the same key-value pairs as `theDict`, or `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## See Also

### Creating a dictionary

func CFDictionaryCreate(CFAllocator!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!, CFIndex, UnsafePointer&lt;CFDictionaryKeyCallBacks>!, UnsafePointer&lt;CFDictionaryValueCallBacks>!) -> CFDictionary!

Creates an immutable dictionary containing the specified key-value pairs.

