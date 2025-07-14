

- XPC
- XPCArray
-  XPCArray.IndexValuePair 

Type Alias

# XPCArray.IndexValuePair

A type that contains an index and the object at that index.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
typealias IndexValuePair = (index: Int, value: xpc_object_t)
```

## Discussion

XPCArray exposes its values as instances of xpc_object_t even if they were originally set with other types.

