

- XPC
-  xpc_date_create(\_:) 

Function

# xpc_date_create(\_:)

Creates an XPC date object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_date_create(_ interval: Int64) -> xpc_object_t
```

## Parameters 

`interval`  

The date interval which is to be boxed. Negative values indicate the number of nanoseconds before the epoch. Positive values indicate the number of nanoseconds after the epoch.

## Return Value

A new date object.

## See Also

### Date objects

func xpc_date_create_from_current() -> xpc_object_t

Creates an XPC date object that represents the current date.

func xpc_date_get_value(xpc_object_t) -> Int64

Returns the underlying date interval from an object.

