

- Endpoint Security
-  es_result_type_t 

Structure

# es_result_type_t

A type that indicates the type of a message’s result.

Mac CatalystmacOS

``` source
struct es_result_type_t
```

## Topics

### Result Types

var ES_RESULT_TYPE_AUTH: es_result_type_t

The authorization result type.

var ES_RESULT_TYPE_FLAGS: es_result_type_t

The flags result type.

### Initializers

init(UInt32)

init(rawValue: UInt32)

### Instance Properties

var rawValue: UInt32

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting Result Properties

var result: es_result_t.__Unnamed_union_result

The message’s result, as either an authorization result or flags.

var result_type: es_result_type_t

The type of the message’s result.

