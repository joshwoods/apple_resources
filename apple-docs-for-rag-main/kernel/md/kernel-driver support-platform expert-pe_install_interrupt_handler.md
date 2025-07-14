

- Kernel
- Driver Support
- Platform Expert
-  PE_install_interrupt_handler 

Function

# PE_install_interrupt_handler

macOS 10.0+

``` source
void PE_install_interrupt_handler(void *nub, int source, void *target, IOInterruptHandler handler, void *refCon);
```

## See Also

### Setup and Initialization

PE_init_cpu

PE_init_iokit

PE_init_panicheader

PE_init_platform

PE_init_printf

PE_init_taproot

PE_boot_args

PE_parse_boot_argn

PE_initialize_console

PE_create_console

PE_current_console

