

- Kernel
- Kernel Functions
-  thread_get_exception_ports_info 

Function

# thread_get_exception_ports_info

macOS 11.3+

``` source
kern_return_t thread_get_exception_ports_info(mach_port_t port, exception_mask_t exception_mask, exception_mask_array_t masks, mach_msg_type_number_t *masksCnt, exception_handler_info_array_t old_handlers_info, exception_behavior_array_t old_behaviors, exception_flavor_array_t old_flavors);
```

