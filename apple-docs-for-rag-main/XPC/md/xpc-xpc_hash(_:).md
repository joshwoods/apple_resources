

- XPC
-  xpc_hash(\_:) 

Function

# xpc_hash(\_:)

Calculates a hash value for the specified object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_hash(_ object: xpc_object_t) -> Int
```

## Parameters 

`object`  

The object for which to calculate a hash value. This value may be modded with a table size for insertion into a dictionary-like data structure.

## Return Value

The calculated hash value.

## Discussion

Note that the computed hash values for any particular type and value of an object can change from across releases and platforms and should not be assumed to be constant across all time and space or stored persistently.

## See Also

### Identity

func xpc_get_type(xpc_object_t) -> xpc_type_t

Returns the type of an object.

func xpc_type_get_name(xpc_type_t) -> UnsafePointer&lt;CChar>

Returns a string that describes an XPC object type.

