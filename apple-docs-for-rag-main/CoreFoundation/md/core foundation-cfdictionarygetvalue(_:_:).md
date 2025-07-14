

- Core Foundation
-  CFDictionaryGetValue(\_:\_:) 

Function

# CFDictionaryGetValue(\_:\_:)

Returns the value associated with a given key.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDictionaryGetValue(
    _ theDict: CFDictionary!,
    _ key: UnsafeRawPointer!
) -> UnsafeRawPointer!
```

## Parameters 

`theDict`  

The dictionary to examine.

`key`  

The key for which to find a match in `theDict`. The key hash and equal callbacks provided when the dictionary was created are used to compare. If the hash callback was `NULL`, the key is treated as a pointer and converted to an integer. If the equal callback was `NULL`, pointer equality (in C, ==) is used. If `key`, or any of the keys in `theDict`, is not understood by the equal callback, the behavior is undefined.

## Return Value

The value associated with `key` in `theDict`, or `NULL` if no key-value pair matching `key` exists. Since `NULL` is also a valid value in some dictionaries, use CFDictionaryGetValueIfPresent(_:_:_:) to distinguish between a value that is not found, and a `NULL` value. If the value is a Core Foundation object, ownership follows the The Get Rule.

## See Also

### Examining a dictionary

func CFDictionaryContainsKey(CFDictionary!, UnsafeRawPointer!) -> Bool

Returns a Boolean value that indicates whether a given key is in a dictionary.

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

func CFDictionaryGetValueIfPresent(CFDictionary!, UnsafeRawPointer!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!) -> Bool

Returns a Boolean value that indicates whether a given value for a given key is in a dictionary, and returns that value indirectly if it exists.

