

- Core Foundation
-  CFDictionaryContainsKey(\_:\_:) 

Function

# CFDictionaryContainsKey(\_:\_:)

Returns a Boolean value that indicates whether a given key is in a dictionary.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDictionaryContainsKey(
    _ theDict: CFDictionary!,
    _ key: UnsafeRawPointer!
) -> Bool
```

## Parameters 

`theDict`  

The dictionary to examine.

`key`  

The key for which to find matches in `theDict`. The key hash and equal callbacks provided when the dictionary was created, are used to compare. If the hash callback is `NULL`, `key` is treated as a pointer and converted to an integer. If the equal callback is `NULL`, pointer equality (in C, ==) is used. If `key`, or any of the keys in the dictionary, is not understood by the equal callback, the behavior is undefined.

## Return Value

`true` if `key` is in the dictionary, otherwise `false`.

## See Also

### Examining a dictionary

func CFDictionaryContainsValue(CFDictionary!, UnsafeRawPointer!) -> Bool

Returns a Boolean value that indicates whether a given value is in a dictionary.

func CFDictionaryGetCount(CFDictionary!) -> CFIndex

Returns the number of key-value pairs in a dictionary.

func CFDictionaryGetCountOfKey(CFDictionary!, UnsafeRawPointer!) -> CFIndex

Returns the number of times a key occurs in a dictionary.

func CFDictionaryGetCountOfValue(CFDictionary!, UnsafeRawPointer!) -> CFIndex

Counts the number of times a given value occurs in the dictionary.

func CFDictionaryGetKeysAndValues(CFDictionary!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!)

Fills two buffers with the keys and values from a dictionary.

func CFDictionaryGetValue(CFDictionary!, UnsafeRawPointer!) -> UnsafeRawPointer!

Returns the value associated with a given key.

func CFDictionaryGetValueIfPresent(CFDictionary!, UnsafeRawPointer!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!) -> Bool

Returns a Boolean value that indicates whether a given value for a given key is in a dictionary, and returns that value indirectly if it exists.

