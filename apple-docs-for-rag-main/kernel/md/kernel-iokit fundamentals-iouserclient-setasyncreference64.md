

- Kernel
- IOKit Fundamentals
- IOUserClient
-  setAsyncReference64 

Type Method

# setAsyncReference64

macOS 10.15.2+

``` source
static void setAsyncReference64(OSAsyncReference64 asyncRef, mach_port_t wakePort, mach_vm_address_t callback, io_user_reference_t refcon, task_t task);
```

