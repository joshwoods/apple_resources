

- Endpoint Security
-  es_result_t 

Structure

# es_result_t

The result of the Endpoint Security subsystem authorization process.

Mac CatalystmacOS

``` source
struct es_result_t
```

## Topics

### Inspecting Result Properties

var result: es_result_t.__Unnamed_union_result

The message’s result, as either an authorization result or flags.

var result_type: es_result_type_t

The type of the message’s result.

struct es_result_type_t

A type that indicates the type of a message’s result.

### Initializers

init()

init(result_type: es_result_type_t, result: es_result_t.__Unnamed_union_result)

## Relationships

### Conforms To

- Sendable

## See Also

### Supporting Types

struct es_string_token_t

A pointer to a null-terminated string, and the length in bytes of that string.

struct es_token_t

An arbitrary buffer of data with its size.

