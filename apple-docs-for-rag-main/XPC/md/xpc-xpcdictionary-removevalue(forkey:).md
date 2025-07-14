

- XPC
- XPCDictionary
-  removeValue(forKey:) 

Instance Method

# removeValue(forKey:)

Removes the given key and its associated value from the dictionary.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
@discardableResult
func removeValue(forKey key: String) -> xpc_object_t?
```

## Parameters 

`key`  

The key to remove along with its associated value.

## Return Value

The value that was removed, or nil if the key was not present in the dictionary.

