

- Security
- cssm_memory_funcs
-  init(malloc_func:free_func:realloc_func:calloc_func:AllocRef:) 

Initializer

# init(malloc_func:free_func:realloc_func:calloc_func:AllocRef:)

Mac Catalyst 13.0+macOS 10.0+

``` source
init(
    malloc_func: CSSM_MALLOC!,
    free_func: CSSM_FREE!,
    realloc_func: CSSM_REALLOC!,
    calloc_func: CSSM_CALLOC!,
    AllocRef: UnsafeMutableRawPointer!
)
```

