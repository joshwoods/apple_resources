

- Kernel
- Kernel Data Types
-  sf_unregistered_func 

Type Alias

# sf_unregistered_func

macOS 10.4+

``` source
typedef void (*sf_unregistered_func)(sflt_handle handle);
```

## Parameters 

`handle`  

The socket filter handle used to identify this filter.

## Discussion

sf_unregistered_func is called to notify the filter it has been unregistered. This is the last function the stack will call and this function will only be called once all other function calls in to your filter have completed. Once this function has been called, your kext may safely unload.

