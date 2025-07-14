

- XPC
-  xpc_bool_get_value(\_:) 

Function

# xpc_bool_get_value(\_:)

Returns the underlying Boolean value from the object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_bool_get_value(_ xbool: xpc_object_t) -> Bool
```

## Parameters 

`xbool`  

The Boolean object which is to be examined.

## Return Value

The underlying Boolean value.

## See Also

### Boolean objects

func xpc_bool_create(Bool) -> xpc_object_t

Creates an XPC Boolean object.

var XPC_BOOL_TRUE: xpc_object_t

A constant that represents a Boolean value of true.

var XPC_BOOL_FALSE: xpc_object_t

A constant that represents a Boolean value of false.

