

- Kernel
- Driver Support
- Platform Expert
-  PE_parse_boot_argn 

Function

# PE_parse_boot_argn

macOS 10.4+

``` source
boolean_t PE_parse_boot_argn(const char *arg_string, void *arg_ptr, int max_arg);
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

PE_initialize_console

PE_install_interrupt_handler

PE_create_console

PE_current_console

