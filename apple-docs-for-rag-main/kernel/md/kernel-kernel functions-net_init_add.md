

- Kernel
- Kernel Functions
-  net_init_add 

Function

# net_init_add

macOS 10.4+

``` source
errno_t net_init_add(net_init_func_ptr init_func);
```

## Parameters 

`init_func`  

A pointer to a function to be called when the stack is initialized.

## Return Value

EINVAL - the init_func value was NULL. EALREADY - the network has already been initialized ENOMEM - there was not enough memory to perform this operation 0 - success

## Discussion

Add a function to be called during network initialization. Your kext must not unload until the function you register is called if net_init_add returns success.

