

- Kernel
- Kernel Data Types
-  kev_msg 

# kev_msg

macOS 10.9+

``` source
struct kev_msg {
    ...
};
```

## Discussion

This structure is used when posting a kernel event.

## Topics

### Fields

vendor_code

The vendor code assigned by kev_vendor_code_find.

kev_class

The event's class.

dv

An array of vectors describing additional data to be appended to the kernel event.

### Instance Properties

event_code

The event's code.

kev_subclass

The event's subclass.

