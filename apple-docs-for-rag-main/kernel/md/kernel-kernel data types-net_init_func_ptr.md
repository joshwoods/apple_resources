

- Kernel
- Kernel Data Types
-  net_init_func_ptr 

Type Alias

# net_init_func_ptr

macOS 10.4+

``` source
typedef void (*net_init_func_ptr)(void);
```

## Discussion

net_init_func_ptr will be called once the networking stack initialized and before network operations occur.

