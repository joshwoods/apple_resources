

- System Configuration
-  SCDynamicStoreSetValue(\_:\_:\_:) 

Function

# SCDynamicStoreSetValue(\_:\_:\_:)

Adds or replaces a value in the dynamic store for the specified key.

macOS 10.1+

``` source
func SCDynamicStoreSetValue(
    _ store: SCDynamicStore?,
    _ key: CFString,
    _ value: CFPropertyList
) -> Bool
```

## Parameters 

`store`  

The dynamic store session.

`key`  

The key associated with the value.

`value`  

The value to add to or replace in the dynamic store.

## Return Value

`TRUE` if the key was updated; otherwise, `FALSE`.

## See Also

### Adding or Updating Keys and Values

func SCDynamicStoreAddTemporaryValue(SCDynamicStore, CFString, CFPropertyList) -> Bool

Temporarily adds the specified key-value pair to the dynamic store, if no such key already exists.

func SCDynamicStoreAddValue(SCDynamicStore?, CFString, CFPropertyList) -> Bool

Adds the specified key-value pair to the dynamic store, if no such key already exists.

func SCDynamicStoreSetMultiple(SCDynamicStore?, CFDictionary?, CFArray?, CFArray?) -> Bool

Updates multiple values in the dynamic store.

