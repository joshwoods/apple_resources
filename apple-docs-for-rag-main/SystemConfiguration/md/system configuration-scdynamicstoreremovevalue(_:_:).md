

- System Configuration
-  SCDynamicStoreRemoveValue(\_:\_:) 

Function

# SCDynamicStoreRemoveValue(\_:\_:)

Removes the value of the specified key from the dynamic store.

macOS 10.1+

``` source
func SCDynamicStoreRemoveValue(
    _ store: SCDynamicStore?,
    _ key: CFString
) -> Bool
```

## Parameters 

`store`  

The dynamic store session.

`key`  

The key of the value to remove.

## Return Value

`TRUE` if the key was removed; `FALSE` if no value was located or an error occurred.

