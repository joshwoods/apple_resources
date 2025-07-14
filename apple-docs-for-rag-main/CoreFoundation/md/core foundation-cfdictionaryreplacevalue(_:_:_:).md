

- Core Foundation
-  CFDictionaryReplaceValue(\_:\_:\_:) 

Function

# CFDictionaryReplaceValue(\_:\_:\_:)

Replaces a value corresponding to a given key.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDictionaryReplaceValue(
    _ theDict: CFMutableDictionary!,
    _ key: UnsafeRawPointer!,
    _ value: UnsafeRawPointer!
)
```

## Parameters 

`theDict`  

The dictionary to modify.

`key`  

The key of the value to replace in `theDict`. If a key which matches `key` is present in the dictionary, the value is changed to the `value`, otherwise this function does nothing (“replace if present”).

`value`  

The new value for `key`. The `value` object is retained by `theDict` using the retain callback provided when `theDict` was created, and the old value is released. `value` must be of the type expected by the retain and release callbacks.

## See Also

### Modifying a Dictionary

func CFDictionaryAddValue(CFMutableDictionary!, UnsafeRawPointer!, UnsafeRawPointer!)

Adds a key-value pair to a dictionary if the specified key is not already present.

func CFDictionaryRemoveAllValues(CFMutableDictionary!)

Removes all the key-value pairs from a dictionary, making it empty.

func CFDictionaryRemoveValue(CFMutableDictionary!, UnsafeRawPointer!)

Removes a key-value pair.

func CFDictionarySetValue(CFMutableDictionary!, UnsafeRawPointer!, UnsafeRawPointer!)

Sets the value corresponding to a given key.

