

- Kernel
- Kernel Data Types
-  backtrace_user_copy_fn 

Type Alias

# backtrace_user_copy_fn

macOS 12.0+

``` source
typedef errno_t (*backtrace_user_copy_fn)(void *ctx, void *dst, user_addr_t src, size_t size);
```

