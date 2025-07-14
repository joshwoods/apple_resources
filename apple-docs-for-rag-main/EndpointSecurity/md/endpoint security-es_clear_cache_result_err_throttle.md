

- Endpoint Security
-  ES_CLEAR_CACHE_RESULT_ERR_THROTTLE 

Global Variable

# ES_CLEAR_CACHE_RESULT_ERR_THROTTLE

Clearing the cache failed because the rate of calls was too high.

Mac CatalystmacOS

``` source
var ES_CLEAR_CACHE_RESULT_ERR_THROTTLE: es_clear_cache_result_t { get }
```

## Discussion

If you receive this response, slow down the rate at which you make calls to es_clear_cache(_:).

## See Also

### Errors

var ES_CLEAR_CACHE_RESULT_ERR_INTERNAL: es_clear_cache_result_t

Communication with the Endpoint Security system failed.

