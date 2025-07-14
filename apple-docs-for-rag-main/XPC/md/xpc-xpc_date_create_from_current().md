

- XPC
-  xpc_date_create_from_current() 

Function

# xpc_date_create_from_current()

Creates an XPC date object that represents the current date.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_date_create_from_current() -> xpc_object_t
```

## Return Value

A new date object representing the current date.

## See Also

### Date objects

func xpc_date_create(Int64) -> xpc_object_t

Creates an XPC date object.

func xpc_date_get_value(xpc_object_t) -> Int64

Returns the underlying date interval from an object.

