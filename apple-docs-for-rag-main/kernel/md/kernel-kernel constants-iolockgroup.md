

- Kernel
- Kernel Constants
-  IOLockGroup 

Global Variable

# IOLockGroup

macOS 10.4+

``` source
lck_grp_t *IOLockGroup;
```

## Discussion

Global lock group used by all IOKit locks. To simplify kext debugging and lock-heat analysis, consider using lck\_\* locks with a per-driver lock group, as defined in kern/locks.h.

