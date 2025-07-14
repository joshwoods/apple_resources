

- System Configuration
-  SCDynamicStoreCopyMultiple(\_:\_:\_:) 

Function

# SCDynamicStoreCopyMultiple(\_:\_:\_:)

Returns the key-value pairs that match the specified keys and key patterns.

macOS 10.1+

``` source
func SCDynamicStoreCopyMultiple(
    _ store: SCDynamicStore?,
    _ keys: CFArray?,
    _ patterns: CFArray?
) -> CFDictionary?
```

## Parameters 

`store`  

The dynamic store session.

`keys`  

The keys associated with the desired values or `NULL` if no specific keys are requested.

`patterns`  

An array of regex(3) pattern strings used to match the keys, or `NULL` if no key patterns are requested.

## Return Value

A dictionary of key-value pairs that match the specified keys and key patterns, or `NULL` if an error occurred. You must release the returned value.

## See Also

### Getting Keys and Values

func SCDynamicStoreCopyKeyList(SCDynamicStore?, CFString) -> CFArray?

Returns the keys that represent the current dynamic store entries that match the specified pattern.

func SCDynamicStoreCopyNotifiedKeys(SCDynamicStore) -> CFArray?

Returns the keys that have changed since the last call to this function.

func SCDynamicStoreCopyValue(SCDynamicStore?, CFString) -> CFPropertyList?

Returns the value associated with the specified key.

