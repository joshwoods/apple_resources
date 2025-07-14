

- Kernel
- Kernel Data Types
-  sockaddr_ctl 

# sockaddr_ctl

macOS 10.13+

``` source
struct sockaddr_ctl {
    ...
};
```

## Discussion

The controller address structure is used to establish contact between a user client and a kernel controller. The sc_id/sc_unit uniquely identify each controller. sc_id is a unique identifier assigned to the controller. The identifier can be assigned by the system at registration time or be a 32-bit creator code obtained from Apple Computer. sc_unit is a unit number for this sc_id, and is privately used by the kernel controller to identify several instances of the controller.

## Topics

### Fields

sc_len

The length of the structure.

sc_family

AF_SYSTEM.

ss_sysaddr

AF_SYS_KERNCONTROL.

sc_id

Controller unique identifier.

sc_unit

Kernel controller private unit number.

sc_reserved

Reserved, must be set to zero.

