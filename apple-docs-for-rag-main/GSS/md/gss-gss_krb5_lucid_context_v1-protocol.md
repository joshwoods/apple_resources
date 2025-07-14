

- GSS
- gss_krb5_lucid_context_v1
-  protocol 

Instance Property

# protocol

The protocol to use.

Mac Catalyst 13.0+macOS 10.14+

``` source
var `protocol`: OM_uint32
```

## Discussion

If this value is 0, then the protocol under RFC-1964 is used. If the value is 1, then the protocol under draft-ietf-krb-wg-gssapi-cfx-07 is used.

## See Also

### Context Members

var cfx_kd: gss_krb5_cfx_keydata_t

The key data structure for Kerberos 5.

var endtime: OM_uint32

The expiration time of the context.

var initiate: OM_uint32

The flag indicating if the role is initiator.

var recv_seq: OM_uint64

The receive sequence number.

var rfc1964_kd: gss_krb5_rfc1964_keydata_t

The RFC-1964 key data.

var send_seq: OM_uint64

The send sequence number.

var version: OM_uint32

The structure version number.

