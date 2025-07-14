

- GSS
- gss_krb5_lucid_context_v1
-  cfx_kd 

Instance Property

# cfx_kd

The key data structure for Kerberos 5.

Mac Catalyst 13.0+macOS 10.14+

``` source
var cfx_kd: gss_krb5_cfx_keydata_t
```

## Discussion

Use this structure only if the `protocol` member is set to 1. In that case, the `rfc1964_kd` member contents are invalid and should be zero.

## See Also

### Context Members

var endtime: OM_uint32

The expiration time of the context.

var initiate: OM_uint32

The flag indicating if the role is initiator.

var `protocol`: OM_uint32

The protocol to use.

var recv_seq: OM_uint64

The receive sequence number.

var rfc1964_kd: gss_krb5_rfc1964_keydata_t

The RFC-1964 key data.

var send_seq: OM_uint64

The send sequence number.

var version: OM_uint32

The structure version number.

