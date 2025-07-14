

- XPC
- XPCArray
-  init(\_:) 

Initializer

# init(\_:)

Creates a new array that contains the given XPC object.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
init(_ value: xpc_object_t)
```

## Parameters 

`value`  

An XPC object. The object’s type must be XPC_TYPE_ARRAY.

## See Also

### Creating an array

init()

Creates a new, empty array.

func copy(into: XPCArray)

Copies the elements of the array to a different array.

