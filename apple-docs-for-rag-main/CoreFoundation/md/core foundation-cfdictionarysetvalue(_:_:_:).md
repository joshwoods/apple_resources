

- Core Foundation
-  CFDictionarySetValue(\_:\_:\_:) 

Function

# CFDictionarySetValue(\_:\_:\_:)

Sets the value corresponding to a given key.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDictionarySetValue(
    _ theDict: CFMutableDictionary!,
    _ key: UnsafeRawPointer!,
    _ value: UnsafeRawPointer!
)
```

## Parameters 

`theDict`  

The dictionary to modify. If this parameter is a fixed-capacity dictionary and it is full before this operation, and the key does not exist in the dictionary, the behavior is undefined.

`key`  

The key of the value to set in `theDict`. If a key which matches `key` is already present in the dictionary, only the value for the key is changed (“add if absent, replace if present”). If no key matches `key`, the key-value pair is added to the dictionary.

If a key-value pair is added, both `key` and `value` are retained by the dictionary, using the retain callback provided when `theDict` was created. `key` must be of the type expected by the key retain callback.

`value`  

The value to add to or replace in `theDict`. `value` is retained using the value retain callback provided when `theDict` was created, and the previous value if any is released. `value` must be of the type expected by the retain and release callbacks.

## See Also

### Modifying a Dictionary

func CFDictionaryAddValue(CFMutableDictionary!, UnsafeRawPointer!, UnsafeRawPointer!)

Adds a key-value pair to a dictionary if the specified key is not already present.

func CFDictionaryRemoveAllValues(CFMutableDictionary!)

Removes all the key-value pairs from a dictionary, making it empty.

func CFDictionaryRemoveValue(CFMutableDictionary!, UnsafeRawPointer!)

Removes a key-value pair.

func CFDictionaryReplaceValue(CFMutableDictionary!, UnsafeRawPointer!, UnsafeRawPointer!)

Replaces a value corresponding to a given key.

