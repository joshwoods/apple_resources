

- Kernel
- Kernel Functions
-  check_task_access_with_flavor 

Function

# check_task_access_with_flavor

macOS 11.3+

``` source
kern_return_t check_task_access_with_flavor(mach_port_t task_access_port, int32_t calling_pid, uint32_t calling_gid, int32_t target_pid, mach_task_flavor_t flavor, audit_token_t caller_cred);
```

