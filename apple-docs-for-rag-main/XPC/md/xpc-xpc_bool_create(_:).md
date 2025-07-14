

- XPC
-  xpc_bool_create(\_:) 

Function

# xpc_bool_create(\_:)

Creates an XPC Boolean object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_bool_create(_ value: Bool) -> xpc_object_t
```

## Parameters 

`value`  

The Boolean primitive value which is to be boxed.

## Return Value

A new Boolean object.

## See Also

### Boolean objects

func xpc_bool_get_value(xpc_object_t) -> Bool

Returns the underlying Boolean value from the object.

var XPC_BOOL_TRUE: xpc_object_t

A constant that represents a Boolean value of true.

var XPC_BOOL_FALSE: xpc_object_t

A constant that represents a Boolean value of false.

