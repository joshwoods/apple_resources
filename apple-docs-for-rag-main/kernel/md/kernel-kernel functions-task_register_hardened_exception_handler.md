

- Kernel
- Kernel Functions
-  task_register_hardened_exception_handler 

Function

# task_register_hardened_exception_handler

macOS 15.0+

``` source
kern_return_t task_register_hardened_exception_handler(task_t task, uint32_t signed_pc_key, exception_mask_t exceptions_allowed, exception_behavior_t behaviors_allowed, thread_state_flavor_t flavors_allowed, mach_port_t new_exception_port);
```

