

- XPC
-  xpc_int64_create(\_:) 

Function

# xpc_int64_create(\_:)

Creates an XPC signed integer object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_int64_create(_ value: Int64) -> xpc_object_t
```

## Parameters 

`value`  

The signed integer value which is to be boxed.

## Return Value

A new signed integer object.

## See Also

### Number objects

func xpc_double_create(Double) -> xpc_object_t

Creates an XPC double object.

func xpc_double_get_value(xpc_object_t) -> Double

Returns the underlying double-precision floating point value from an object.

func xpc_int64_get_value(xpc_object_t) -> Int64

Returns the underlying signed 64-bit integer value from an object.

func xpc_uint64_create(UInt64) -> xpc_object_t

Creates an XPC unsigned integer object.

func xpc_uint64_get_value(xpc_object_t) -> UInt64

Returns the underlying unsigned 64-bit integer value from an object.

