

- XPC
-  XPC_BOOL_FALSE 

Global Variable

# XPC_BOOL_FALSE

A constant that represents a Boolean value of false.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOS 9.0+watchOS 2.0+

``` source
var XPC_BOOL_FALSE: xpc_object_t { get }
```

## Discussion

You may compare a Boolean object against this constant to determine its value.

## See Also

### Boolean objects

func xpc_bool_create(Bool) -> xpc_object_t

Creates an XPC Boolean object.

func xpc_bool_get_value(xpc_object_t) -> Bool

Returns the underlying Boolean value from the object.

var XPC_BOOL_TRUE: xpc_object_t

A constant that represents a Boolean value of true.

