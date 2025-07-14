

- Kernel
- mach
-  mach_gss_accept_sec_context 

Function

# mach_gss_accept_sec_context

macOS 10.5+

``` source
kern_return_t mach_gss_accept_sec_context(mach_port_t server, gssd_byte_buffer intoken, mach_msg_type_number_t intokenCnt, gssd_string svc_namestr, uint32_t gssd_flags, gssd_ctx *context, gssd_cred *cred_handle, uint32_t *flags, uint32_t *uid, gssd_gid_list gids, mach_msg_type_number_t *gidsCnt, gssd_byte_buffer *key, mach_msg_type_number_t *keyCnt, gssd_byte_buffer *outtoken, mach_msg_type_number_t *outtokenCnt, uint32_t *major_stat, uint32_t *minor_stat);
```

## See Also

### Security

mach_gss_accept_sec_context_v2

mach_gss_hold_cred

mach_gss_init_sec_context

mach_gss_init_sec_context_v2

mach_gss_init_sec_context_v3

mach_gss_log_error

mach_gss_lookup

mach_gss_unhold_cred

