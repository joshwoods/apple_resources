

- Endpoint Security
-  es_clear_cache_result_t 

Structure

# es_clear_cache_result_t

Values that indicate the result of clearing a cache.

Mac CatalystmacOS

``` source
struct es_clear_cache_result_t
```

## Topics

### Success

var ES_CLEAR_CACHE_RESULT_SUCCESS: es_clear_cache_result_t

Clearing the cache succeeded.

### Errors

var ES_CLEAR_CACHE_RESULT_ERR_INTERNAL: es_clear_cache_result_t

Communication with the Endpoint Security system failed.

var ES_CLEAR_CACHE_RESULT_ERR_THROTTLE: es_clear_cache_result_t

Clearing the cache failed because the rate of calls was too high.

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

### Managing Cached Results

func es_clear_cache(OpaquePointer) -> es_clear_cache_result_t

Clears all cached results for all clients.

