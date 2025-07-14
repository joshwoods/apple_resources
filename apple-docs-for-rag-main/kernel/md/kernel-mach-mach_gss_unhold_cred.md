

- Kernel
- mach
-  mach_gss_unhold_cred 

Function

# mach_gss_unhold_cred

macOS 10.7+

``` source
kern_return_t mach_gss_unhold_cred(mach_port_t server, gssd_mechtype mech, gssd_nametype nt, gssd_byte_buffer princ, mach_msg_type_number_t princCnt, uint32_t *major_stat, uint32_t *minor_stat);
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

mach_gss_lookup

