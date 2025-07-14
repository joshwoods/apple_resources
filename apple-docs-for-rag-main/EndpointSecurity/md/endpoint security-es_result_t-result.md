

- Endpoint Security
- es_result_t
-  result 

Instance Property

# result

The message’s result, as either an authorization result or flags.

Mac CatalystmacOS

``` source
var result: es_result_t.__Unnamed_union_result
```

## Discussion

This type is a `union` of an es_auth_result_t named `auth` and a uint32_t named `flags`. Use the result_type field to determine which type this result represents.

## See Also

### Inspecting Result Properties

var result_type: es_result_type_t

The type of the message’s result.

struct es_result_type_t

A type that indicates the type of a message’s result.

