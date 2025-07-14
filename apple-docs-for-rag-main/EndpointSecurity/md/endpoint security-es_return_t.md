

- Endpoint Security
-  es_return_t 

Structure

# es_return_t

Values that indicate the result of an Endpoint Security action that can only succeed or fail.

Mac CatalystmacOS

``` source
struct es_return_t
```

## Topics

### Return Values

var ES_RETURN_SUCCESS: es_return_t

The action succeeded.

var ES_RETURN_ERROR: es_return_t

The action failed with an error.

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

