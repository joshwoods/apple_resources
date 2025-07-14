

- Endpoint Security
-  es_clear_cache(\_:) 

Function

# es_clear_cache(\_:)

Clears all cached results for all clients.

macOS 10.15+

``` source
func es_clear_cache(_ client: OpaquePointer) -> es_clear_cache_result_t
```

## Parameters 

`client`  

The client that performs the request.

## Discussion

Endpoint Security shares caches across all clients, so you can provide any valid client as the parameter to this function.

## See Also

### Managing Cached Results

struct es_clear_cache_result_t

Values that indicate the result of clearing a cache.

