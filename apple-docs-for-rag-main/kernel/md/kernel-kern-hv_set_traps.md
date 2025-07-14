

- Kernel
- kern
-  hv_set_traps 

Function

# hv_set_traps

macOS 10.10+

``` source
kern_return_t hv_set_traps(hv_trap_type_t trap_type, const hv_trap_t *traps, unsigned int trap_count);
```

## See Also

### hv

hv_ast_pending

hv_get_support

hv_get_task_target

hv_get_thread_target

hv_get_volatile_state

hv_release_callbacks

hv_release_traps

hv_set_callbacks

hv_set_task_target

hv_set_thread_target

hv_support_init

hv_suspend

hv_task_trap

hv_thread_trap

