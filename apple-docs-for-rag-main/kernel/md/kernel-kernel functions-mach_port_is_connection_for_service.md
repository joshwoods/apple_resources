

- Kernel
- Kernel Functions
-  mach_port_is_connection_for_service 

Function

# mach_port_is_connection_for_service

macOS 12.0+

``` source
kern_return_t mach_port_is_connection_for_service(ipc_space_t task, mach_port_name_t connection_port, mach_port_name_t service_port, uint64_t *filter_policy_id);
```

