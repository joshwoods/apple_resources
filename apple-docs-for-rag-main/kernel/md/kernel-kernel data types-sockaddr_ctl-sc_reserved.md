

- Kernel
- Kernel Data Types
- sockaddr_ctl
-  sc_reserved 

Instance Property

# sc_reserved

Reserved, must be set to zero.

macOS 10.13+

``` source
u_int32_t sc_reserved[5];
```

## See Also

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

