

- System Configuration
-  SCDynamicStoreCopyValue(\_:\_:) 

Function

# SCDynamicStoreCopyValue(\_:\_:)

Returns the value associated with the specified key.

macOS 10.1+

``` source
func SCDynamicStoreCopyValue(
    _ store: SCDynamicStore?,
    _ key: CFString
) -> CFPropertyList?
```

## Parameters 

`store`  

The dynamic store session.

`key`  

The key associated with the desired value.

## Return Value

The value associated with the specified key, or `NULL` if no value was located or if an error occurred. You must release the returned value.

## See Also

### Getting Keys and Values

func SCDynamicStoreCopyKeyList(SCDynamicStore?, CFString) -> CFArray?

Returns the keys that represent the current dynamic store entries that match the specified pattern.

func SCDynamicStoreCopyMultiple(SCDynamicStore?, CFArray?, CFArray?) -> CFDictionary?

Returns the key-value pairs that match the specified keys and key patterns.

func SCDynamicStoreCopyNotifiedKeys(SCDynamicStore) -> CFArray?

Returns the keys that have changed since the last call to this function.

