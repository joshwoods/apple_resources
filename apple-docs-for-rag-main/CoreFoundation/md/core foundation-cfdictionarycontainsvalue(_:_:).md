

- Core Foundation
-  CFDictionaryContainsValue(\_:\_:) 

Function

# CFDictionaryContainsValue(\_:\_:)

Returns a Boolean value that indicates whether a given value is in a dictionary.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDictionaryContainsValue(
    _ theDict: CFDictionary!,
    _ value: UnsafeRawPointer!
) -> Bool
```

## Parameters 

`theDict`  

The dictionary to examine.

`value`  

The value for which to find matches in `theDict`. The value equal callback provided when the dictionary was created is used to compare. If the equal callback was `NULL`, pointer equality (in C, ==) is used. If `value`, or any other value in the dictionary, is not understood by the equal callback, the behavior is undefined.

## Return Value

`true` if `value` is in the dictionary, otherwise `false`.

## See Also

### Examining a dictionary

func CFDictionaryContainsKey(CFDictionary!, UnsafeRawPointer!) -> Bool

Returns a Boolean value that indicates whether a given key is in a dictionary.

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

