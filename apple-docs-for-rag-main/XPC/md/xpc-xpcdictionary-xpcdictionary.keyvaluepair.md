

- XPC
- XPCDictionary
-  XPCDictionary.KeyValuePair 

Type Alias

# XPCDictionary.KeyValuePair

A type that contains a dictionary’s key-value pair.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
typealias KeyValuePair = (key: String, value: xpc_object_t)
```

## Discussion

XPCDictionary exposes its values as instances of xpc_object_t even if they were originally set with other types.

