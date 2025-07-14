

- XPC
- XPCArray
-  forEach(\_:) 

Instance Method

# forEach(\_:)

Calls the given closure with an index and element of the array in the same order as a for-in loop.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
func forEach(_ body: (Int, xpc_object_t) throws -> Void) rethrows
```

## Parameters 

`body`  

A closure that takes an index and an element of the sequence as parameters.

## See Also

### Iterating over an array’s elements

func forEach((XPCArray.IndexValuePair) throws -> Void) rethrows

Calls the given closure with each element in the array in the same order as a for-in loop.

