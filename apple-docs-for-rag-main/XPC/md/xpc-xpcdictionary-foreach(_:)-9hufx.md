

- XPC
- XPCDictionary
-  forEach(\_:) 

Instance Method

# forEach(\_:)

Calls the given closure with each element in the dictionary in the same order as a for-in loop.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
func forEach(_ body: (XPCDictionary.KeyValuePair) throws -> Void) rethrows
```

## Parameters 

`body`  

A closure that takes an element of the sequence as a parameter.

## See Also

### Iterating over keys and values

func forEach((String, xpc_object_t) throws -> Void) rethrows

Calls the given closure with each key and value in the dictionary in the same order as a for-in loop.

