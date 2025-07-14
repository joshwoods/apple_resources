

- Kernel
- Kernel Data Types
-  kern_ctl_ref 

Type Alias

# kern_ctl_ref

macOS 10.13+

``` source
typedef void *kern_ctl_ref;
```

## Discussion

A control reference is used to track an attached kernel control. Registering a kernel control will create a kernel control reference. This reference is required for sending data or removing the kernel control. This reference will be passed to callbacks for that kernel control.

