

- Core Foundation
-  CFDictionaryGetKeysAndValues(\_:\_:\_:) 

Function

# CFDictionaryGetKeysAndValues(\_:\_:\_:)

Fills two buffers with the keys and values from a dictionary.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDictionaryGetKeysAndValues(
    _ theDict: CFDictionary!,
    _ keys: UnsafeMutablePointer!,
    _ values: UnsafeMutablePointer!
)
```

## Parameters 

`theDict`  

The dictionary to examine.

`keys`  

A C array of pointer-sized values that, on return, is filled with keys from the `theDict`. The keys and values C arrays are parallel to each other (that is, the items at the same indices form a key-value pair from the dictionary). This value must be a valid pointer to a C array of the appropriate type and size (that is, a size equal to the count of `theDict`), or `NULL` if the keys are not required. If the keys are Core Foundation objects, ownership follows the The Get Rule.

`values`  

A C array of pointer-sized values that, on return, is filled with values from the `theDict`. The keys and values C arrays are parallel to each other (that is, the items at the same indices form a key-value pair from the dictionary). This value must be a valid pointer to a C array of the appropriate type and size (that is, a size equal to the count of `theDict`), or `NULL` if the values are not required. If the values are Core Foundation objects, ownership follows the The Get Rule.

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

func CFDictionaryGetValue(CFDictionary!, UnsafeRawPointer!) -> UnsafeRawPointer!

Returns the value associated with a given key.

func CFDictionaryGetValueIfPresent(CFDictionary!, UnsafeRawPointer!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!) -> Bool

Returns a Boolean value that indicates whether a given value for a given key is in a dictionary, and returns that value indirectly if it exists.

