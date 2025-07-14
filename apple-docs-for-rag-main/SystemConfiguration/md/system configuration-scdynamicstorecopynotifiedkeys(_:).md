

- System Configuration
-  SCDynamicStoreCopyNotifiedKeys(\_:) 

Function

# SCDynamicStoreCopyNotifiedKeys(\_:)

Returns the keys that have changed since the last call to this function.

macOS 10.1+

``` source
func SCDynamicStoreCopyNotifiedKeys(_ store: SCDynamicStore) -> CFArray?
```

## Parameters 

`store`  

The dynamic store session.

## Return Value

The keys that have changed, or `NULL` if an error occurred. You must release the returned value.

## Discussion

If possible, your application should use the notification functions instead of polling for the list of changed keys returned by this function.

## See Also

### Getting Keys and Values

func SCDynamicStoreCopyKeyList(SCDynamicStore?, CFString) -> CFArray?

Returns the keys that represent the current dynamic store entries that match the specified pattern.

func SCDynamicStoreCopyMultiple(SCDynamicStore?, CFArray?, CFArray?) -> CFDictionary?

Returns the key-value pairs that match the specified keys and key patterns.

func SCDynamicStoreCopyValue(SCDynamicStore?, CFString) -> CFPropertyList?

Returns the value associated with the specified key.

