

- Kernel
- Kernel Data Types
-  sysctl_handler_t 

Type Alias

# sysctl_handler_t

macOS 10.5+

``` source
typedef int (*sysctl_handler_t)(struct sysctl_oid *oidp, void *arg1, int arg2, struct sysctl_req *req);
```

