

- XPC
-  xpc_copy(\_:) 

Function

# xpc_copy(\_:)

Creates a copy of the object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_copy(_ object: xpc_object_t) -> xpc_object_t?
```

## Parameters 

`object`  

The object to copy.

## Return Value

The new object. `NULL` if the object type does not support copying or if sufficient memory for the copy could not be allocated. Service objects do not support copying.

## Discussion

When called on an array or dictionary, xpc_copy(_:) will perform a deep copy.

The object returned is not necessarily guaranteed to be a new object, and whether it is will depend on the implementation of the object being copied.

## See Also

### Copying

func xpc_copy_description(xpc_object_t) -> UnsafeMutablePointer&lt;CChar>

Copies a debug string that describes the object.

