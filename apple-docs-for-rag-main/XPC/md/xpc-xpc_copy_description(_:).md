

- XPC
-  xpc_copy_description(\_:) 

Function

# xpc_copy_description(\_:)

Copies a debug string that describes the object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_copy_description(_ object: xpc_object_t) -> UnsafeMutablePointer
```

## Parameters 

`object`  

The object which is to be examined.

## Return Value

A string describing object which contains information useful for debugging. This string should be disposed of with `free(3)` when done.

## See Also

### Copying

func xpc_copy(xpc_object_t) -> xpc_object_t?

Creates a copy of the object.

