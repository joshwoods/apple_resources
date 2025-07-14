

- GSS
- gss_krb5_lucid_context_v1
-  init(version:initiate:endtime:send_seq:recv_seq:protocol:rfc1964_kd:cfx_kd:) 

Initializer

# init(version:initiate:endtime:send_seq:recv_seq:protocol:rfc1964_kd:cfx_kd:)

Mac Catalyst 13.0+macOS 10.14+

``` source
init(
    version: OM_uint32,
    initiate: OM_uint32,
    endtime: OM_uint32,
    send_seq: OM_uint64,
    recv_seq: OM_uint64,
    protocol: OM_uint32,
    rfc1964_kd: gss_krb5_rfc1964_keydata_t,
    cfx_kd: gss_krb5_cfx_keydata_t
)
```

