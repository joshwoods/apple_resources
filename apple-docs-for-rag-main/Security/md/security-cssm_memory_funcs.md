

- Security
-  cssm_memory_funcs 

Structure

# cssm_memory_funcs

Mac Catalyst 13.0+macOS 10.0+

``` source
struct cssm_memory_funcs
```

## Topics

### Initializers

init()

init(malloc_func: CSSM_MALLOC!, free_func: CSSM_FREE!, realloc_func: CSSM_REALLOC!, calloc_func: CSSM_CALLOC!, AllocRef: UnsafeMutableRawPointer!)

### Instance Properties

var AllocRef: UnsafeMutableRawPointer!

var calloc_func: CSSM_CALLOC!

var free_func: CSSM_FREE!

var malloc_func: CSSM_MALLOC!

var realloc_func: CSSM_REALLOC!

## Relationships

### Conforms To

- BitwiseCopyable

