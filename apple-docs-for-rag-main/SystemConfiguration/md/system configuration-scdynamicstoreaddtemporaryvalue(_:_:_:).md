

- System Configuration
-  SCDynamicStoreAddTemporaryValue(\_:\_:\_:) 

Function

# SCDynamicStoreAddTemporaryValue(\_:\_:\_:)

Temporarily adds the specified key-value pair to the dynamic store, if no such key already exists.

macOS 10.1+

``` source
func SCDynamicStoreAddTemporaryValue(
    _ store: SCDynamicStore,
    _ key: CFString,
    _ value: CFPropertyList
) -> Bool
```

## Parameters 

`store`  

The dynamic store session.

`key`  

The key of the value to add to the dynamic store.

`value`  

The value to add to the dynamic store.

## Return Value

`TRUE` if the key was added; `FALSE` if the key was already present in the dynamic store or if an error occurred.

## Discussion

Unless the key is updated by another session, the key-value pair added by this function is removed automatically when the session is closed.

## See Also

### Adding or Updating Keys and Values

func SCDynamicStoreAddValue(SCDynamicStore?, CFString, CFPropertyList) -> Bool

Adds the specified key-value pair to the dynamic store, if no such key already exists.

func SCDynamicStoreSetMultiple(SCDynamicStore?, CFDictionary?, CFArray?, CFArray?) -> Bool

Updates multiple values in the dynamic store.

func SCDynamicStoreSetValue(SCDynamicStore?, CFString, CFPropertyList) -> Bool

Adds or replaces a value in the dynamic store for the specified key.

