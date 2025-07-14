

- Kernel
- Kernel Data Types
-  idle_timer_t 

Type Alias

# idle_timer_t

macOS 11.0+

``` source
typedef void (*idle_timer_t)(void *refcon, uint64_t *new_timeout_ticks);
```

