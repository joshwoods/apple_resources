

- Kernel
- mach
-  mach_gss_lookup 

Function

# mach_gss_lookup

macOS 10.8+

``` source
kern_return_t mach_gss_lookup(mach_port_t server, uint32_t uid, int32_t asid, mach_port_t *gssd_session_port);
```

## See Also

### Security

mach_gss_accept_sec_context

mach_gss_accept_sec_context_v2

mach_gss_hold_cred

mach_gss_init_sec_context

mach_gss_init_sec_context_v2

mach_gss_init_sec_context_v3

mach_gss_log_error

mach_gss_unhold_cred

