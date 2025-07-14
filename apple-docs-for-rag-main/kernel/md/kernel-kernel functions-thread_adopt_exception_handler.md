

- Kernel
- Kernel Functions
-  thread_adopt_exception_handler 

Function

# thread_adopt_exception_handler

macOS 15.0+

``` source
kern_return_t thread_adopt_exception_handler(thread_t thread, mach_port_t exc_port, exception_mask_t exc_mask, exception_behavior_t behavior_mask, thread_state_flavor_t flavor_mask);
```

