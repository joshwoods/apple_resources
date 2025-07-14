

- Core Foundation
-  CFDictionaryRemoveValue(\_:\_:) 

Function

# CFDictionaryRemoveValue(\_:\_:)

Removes a key-value pair.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDictionaryRemoveValue(
    _ theDict: CFMutableDictionary!,
    _ key: UnsafeRawPointer!
)
```

## Parameters 

`theDict`  

The dictionary to modify.

`key`  

The key of the value to remove from `theDict`. If a key which matches `key` is present in `theDict`, the key-value pair is removed from the dictionary, otherwise this function does nothing (“remove if present”).

## See Also

### Modifying a Dictionary

func CFDictionaryAddValue(CFMutableDictionary!, UnsafeRawPointer!, UnsafeRawPointer!)

Adds a key-value pair to a dictionary if the specified key is not already present.

func CFDictionaryRemoveAllValues(CFMutableDictionary!)

Removes all the key-value pairs from a dictionary, making it empty.

func CFDictionaryReplaceValue(CFMutableDictionary!, UnsafeRawPointer!, UnsafeRawPointer!)

Replaces a value corresponding to a given key.

func CFDictionarySetValue(CFMutableDictionary!, UnsafeRawPointer!, UnsafeRawPointer!)

Sets the value corresponding to a given key.

