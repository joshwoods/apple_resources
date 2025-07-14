

- System Configuration
-  SCDynamicStoreCopyKeyList(\_:\_:) 

Function

# SCDynamicStoreCopyKeyList(\_:\_:)

Returns the keys that represent the current dynamic store entries that match the specified pattern.

macOS 10.1+

``` source
func SCDynamicStoreCopyKeyList(
    _ store: SCDynamicStore?,
    _ pattern: CFString
) -> CFArray?
```

## Parameters 

`store`  

The dynamic store session.

`pattern`  

A regex(3) regular expression pattern used to match the dynamic store keys.

## Return Value

An array of matching keys, or `NULL` if an error occurred. You must release the returned value.

## See Also

### Getting Keys and Values

func SCDynamicStoreCopyMultiple(SCDynamicStore?, CFArray?, CFArray?) -> CFDictionary?

Returns the key-value pairs that match the specified keys and key patterns.

func SCDynamicStoreCopyNotifiedKeys(SCDynamicStore) -> CFArray?

Returns the keys that have changed since the last call to this function.

func SCDynamicStoreCopyValue(SCDynamicStore?, CFString) -> CFPropertyList?

Returns the value associated with the specified key.

