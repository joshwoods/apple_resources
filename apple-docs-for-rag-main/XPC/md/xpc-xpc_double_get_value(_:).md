

- XPC
-  xpc_double_get_value(\_:) 

Function

# xpc_double_get_value(\_:)

Returns the underlying double-precision floating point value from an object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_double_get_value(_ xdouble: xpc_object_t) -> Double
```

## Parameters 

`xdouble`  

The floating point object which is to be examined.

## Return Value

The underlying floating point value.

## See Also

### Number objects

func xpc_double_create(Double) -> xpc_object_t

Creates an XPC double object.

func xpc_int64_create(Int64) -> xpc_object_t

Creates an XPC signed integer object.

func xpc_int64_get_value(xpc_object_t) -> Int64

Returns the underlying signed 64-bit integer value from an object.

func xpc_uint64_create(UInt64) -> xpc_object_t

Creates an XPC unsigned integer object.

func xpc_uint64_get_value(xpc_object_t) -> UInt64

Returns the underlying unsigned 64-bit integer value from an object.

