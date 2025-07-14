

- Kernel
- Kernel Data Types
-  processor_idle_t 

Type Alias

# processor_idle_t

macOS 11.0+

``` source
typedef void (*processor_idle_t)(cpu_id_t cpu_id, boolean_t enter, uint64_t *new_timeout_ticks);
```

