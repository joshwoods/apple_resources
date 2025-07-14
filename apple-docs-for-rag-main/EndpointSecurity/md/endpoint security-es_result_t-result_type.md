

- Endpoint Security
- es_result_t
-  result_type 

Instance Property

# result_type

The type of the message’s result.

Mac CatalystmacOS

``` source
var result_type: es_result_type_t
```

## Discussion

Use this value to determine which member of the result `union` to use: `auth` or `flags`.

## See Also

### Inspecting Result Properties

var result: es_result_t.__Unnamed_union_result

The message’s result, as either an authorization result or flags.

struct es_result_type_t

A type that indicates the type of a message’s result.

