

- Kernel
- mach
-  mach_gss_log_error 

Function

# mach_gss_log_error

macOS 10.5+

``` source
kern_return_t mach_gss_log_error(mach_port_t server, gssd_string mnt, uint32_t uid, gssd_string source, uint32_t major_stat, uint32_t minor_stat);
```

## See Also

### Security

mach_gss_accept_sec_context

mach_gss_accept_sec_context_v2

mach_gss_hold_cred

mach_gss_init_sec_context

mach_gss_init_sec_context_v2

mach_gss_init_sec_context_v3

mach_gss_lookup

mach_gss_unhold_cred

