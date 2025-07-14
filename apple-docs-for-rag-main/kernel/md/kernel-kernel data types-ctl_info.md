

- Kernel
- Kernel Data Types
-  ctl_info 

# ctl_info

macOS 10.13+

``` source
struct ctl_info {
    ...
};
```

## Discussion

This structure is used with the CTLIOCGINFO ioctl to translate from a kernel control name to a control id.

## Topics

### Fields

ctl_id

The kernel control id, filled out upon return.

ctl_name

The kernel control name to find.

